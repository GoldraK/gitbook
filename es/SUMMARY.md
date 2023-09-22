# Table of contents

* [👋 Introducción](README.md)
  * [Desarrollo](introduccion/desarrollo.md)
  * [Integración Continua (CI)](introduccion/integracion-continua-ci/README.md)
    * [Flujo de trabajo](introduccion/integracion-continua-ci/flujo-de-trabajo.md)
    * [Herramientas](introduccion/integracion-continua-ci/herramientas.md)
  * [Entrega Continua (CD)](introduccion/entrega-continua-cd/README.md)
    * [Flujo de Trabajo](introduccion/entrega-continua-cd/flujo-de-trabajo.md)
    * [Herramientas](introduccion/entrega-continua-cd/herramientas.md)
  * [Monitorización](introduccion/monitorizacion.md)

## Infrastructura

* [Kubernetes (k8s)](infrastructura/kubernetes-k8s.md)
* [Gitlab](infrastructura/gitlab/README.md)
  * [Runner](infrastructura/gitlab/runner.md)
  * [CI/CD](infrastructura/gitlab/ci-cd.md)
* [Harbor](infrastructura/harbor/README.md)
  * [Instalación](infrastructura/harbor/instalacion.md)
* [SonarQube](infrastructura/sonarqube/README.md)
  * [Instalación](infrastructura/sonarqube/instalacion.md)
* [Dependency-Track](infrastructura/dependency-track/README.md)
  * [Instalación](infrastructura/dependency-track/instalacion.md)
* [DefectDojo](infrastructura/defectdojo/README.md)
  * [Instalación](infrastructura/defectdojo/instalacion.md)

## Desarrollo

* [Harbor](desarrollo/harbor.md)
* [Git](desarrollo/git/README.md)
  * [Hooks](desarrollo/git/hooks/README.md)
    * [pre-commit](desarrollo/git/hooks/pre-commit/README.md)
      * [PHP](desarrollo/git/hooks/pre-commit/php.md)

## CI

* [Fugas de Contraseñas](ci/fugas-de-contrasenas/README.md)
  * [Gitleaks](ci/fugas-de-contrasenas/gitleaks/README.md)
    * [Uso](ci/fugas-de-contrasenas/gitleaks/uso.md)
* [SBOM](ci/sbom/README.md)
  * [CyconeDX](ci/sbom/cyconedx/README.md)
    * [PHP](ci/sbom/cyconedx/php.md)
* [Testing](ci/testing/README.md)
  * [PHP](ci/testing/php.md)
* [SAST](ci/sast/README.md)
  * [SonarQube](ci/sast/sonarqube.md)
* [Contenedores](ci/contenedores/README.md)
  * [SAST](ci/contenedores/sast.md)
  * [Construcción](ci/contenedores/construccion.md)
  * [Analisis](ci/contenedores/analisis.md)
  * [Publicación](ci/contenedores/publicacion.md)
  * [Firma](ci/contenedores/firma.md)
* [DAST](ci/dast/README.md)
  * [OWASP ZAP](ci/dast/owasp-zap.md)
* [Integraciones Monitorización](ci/integraciones-monitorizacion.md)

## CD

* [Despliegue](cd/despliegue.md)

## Monitorización

* [Dependency-Track](monitorizacion/dependency-track.md)
* [DefectDojo](monitorizacion/defectdojo/README.md)
  * [Producto](monitorizacion/defectdojo/producto.md)
  * [Engagement](monitorizacion/defectdojo/engagement.md)
  * [Finding](monitorizacion/defectdojo/finding.md)
