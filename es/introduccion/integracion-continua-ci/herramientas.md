# Herramientas

Para llevar a cabo el flujo de trabajo descrito anteriormente, utilizaremos una serie de herramientas que se detallarán en las siguientes fases.

### **Búsqueda de Fugas de Contraseñas**

* Herramienta: Gitleaks
* Explicación: Gitleaks escanea el repositorio de código en busca de posibles fugas de contraseñas y datos sensibles, previniendo la exposición no deseada de información confidencial.

### **Análisis de Dependencias (SBOM)**

* Herramienta: CycloneDx
* Explicación: CycloneDx realiza un análisis exhaustivo de las dependencias del proyecto, proporcionando un panorama claro de las bibliotecas utilizadas y ayudando a identificar vulnerabilidades potenciales.

### **Pruebas Unitarias e Integración**

* Herramienta: PHPUnit
* Explicación: PHPUnit permite la creación y ejecución de pruebas unitarias para validar el funcionamiento correcto de las partes individuales del código, asegurando la integridad del software.

### **Análisis de Código Estático (SAST)**

* Herramienta: SonarQube
* Explicación: SonarQube realiza un análisis estático del código en busca de vulnerabilidades y problemas de calidad, mejorando la seguridad y la calidad del código.

### **Análisis de Dockerfile**

* Herramienta: Hadolint
* Explicación: Hadolint es una herramienta especializada que analiza los Dockerfiles en busca de posibles problemas o configuraciones que puedan comprometer la seguridad en la construcción de imágenes de contenedor.

### **Construcción de Contenedores**

* Herramienta: Docker (docker build)
* Explicación: Docker permite la construcción de imágenes de contenedor mediante el comando "docker build", configurando entornos de ejecución seguros y eficientes.

### **Análisis de Contenedores**

* Herramienta: Trivy
* Explicación: Trivy analiza las imágenes de contenedor en busca de vulnerabilidades en los componentes, proporcionando información sobre posibles riesgos y permitiendo acciones correctivas.

### **Firmado de Contenedores**

* Herramienta: Cosign
* Explicación: Cosign proporciona firmas digitales para los contenedores, asegurando su autenticidad e integridad, lo que refuerza la seguridad y confiabilidad en el despliegue.

### **Análisis Dinámico (DAST)**

* Herramienta: OWASP ZAP
* Explicación: OWASP ZAP realiza análisis dinámicos de seguridad, simulando ataques en tiempo real sobre el código en ejecución para identificar vulnerabilidades y riesgos en el sistema desplegado.
