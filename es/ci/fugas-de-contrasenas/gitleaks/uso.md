# Uso

Podemos integrar Gitleaks con otra de las herramientas disponibles en nuestro flujo de trabajo, que es DefectDojo, para poder visualizar la información de manera cómoda en el panel de control.

### Integración con Gitlab

Para integrar Gitleaks con CI/CD de Gitlab, tenemos dos opciones: utilizar la imagen disponible en el [DockerHub](https://hub.docker.com/r/zricethezav/gitleaks) o la que tenemos en el proyecto [OSDO](https://harbor.opensecdevops.com/harbor/projects/2/repositories/gitleak/artifacts-tab?publicAndNotLogged=yes), que ya tiene instalado Curl para permitir la integración con DefectDojo.

Una vez que hayamos decidido cuál opción necesitamos, procedemos a añadir la siguiente sección en nuestro archivo `gitlab-ci.yml`:

```yaml
secret_detection:
  stage: secret_detection
  variables:
    GIT_STRATEGY: clone
    GIT_DEPTH: 1
  image: 
    name: Image-need
    entrypoint: [""]
  script:
    - gitleaks detect -v --source=$PWD  --report-path=gitleaks-report.json
  artifacts:
    paths:
      - gitleaks-report.json

```

Lo que hacemos con este stage es clonar el último commit nada más, dado que GitLeaks busca en todos los commits y si existía un leak en un commit antiguo con este fallo de seguridad seguiría dando la alerta.

### DefectDojo

Para realizar la integración con DefectDojo, debemos agregar la opción `after_script` en nuestro archivo de configuración de GitLab CI/CD. En este paso, llamaremos al script `defectdojo-finding.sh`", que se encuentra en la sección de "Integraciones de Monitorización". Para asegurarnos de que la llamada al script solo se realice si se han encontrado "leaks", lo envolvemos en una estructura condicional `if` que verifica el estado del trabajo con la variable `$CI_JOB_STATUS`. También debemos agregar las siguientes variables de configuración para personalizar el "finding": `$DD_SCAN_TYPE,` `$DD_PRODUCT_NAME`, `$DD_SCAN_FILE`, `$DD_SCAN_ACTIVE`, `$DD_SCAN_VERIFIED`.

```yaml
secret_detection:
  stage: secret_detection
  dependencies: ["defectdojo_create_engagement"]
  variables:
    GIT_STRATEGY: clone
    GIT_DEPTH: 1
    DD_SCAN_TYPE: "Gitleaks Scan"
    DD_PRODUCT_NAME: "GitLeaks"
    DD_SCAN_FILE: "gitleaks-report.json"
    DD_SCAN_ACTIVE: "true"
    DD_SCAN_VERIFIED: "false"
  image: 
    name: harbor.opensecdevops.com/osdo/gitleak@sha256:d348f3c616c5b51b8e6bb1702484d6f293712be43fc81c3b97793f0886b7f95b
    entrypoint: [""]
  script:
    - gitleaks detect -v --source=$PWD  --report-path=gitleaks-report.json
  after_script:
    - |
      if [ $CI_JOB_STATUS == 'failed' ]; then
        bash .gitlab-ci/defectdojo-finding.sh
      fi
  artifacts:
    when: on_failure
    paths:
      - gitleaks-report.json
```

