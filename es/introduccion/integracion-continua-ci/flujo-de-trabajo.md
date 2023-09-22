# Flujo de trabajo

Con el objetivo de asegurar un proceso de desarrollo seguro dentro de nuestra estructura de trabajo, delinearemos diversas etapas que deben ser implementadas. Es fundamental considerar que estas etapas deben ajustarse a las particularidades de cada proyecto, reconociendo que no todas necesariamente deben ser incorporadas en cada caso. Esto nos proporciona un enfoque flexible y personalizable para alcanzar niveles óptimos de seguridad en cada proyecto individual.

### **Búsqueda de Fugas de Contraseñas**

En esta fase, utilizaremos una herramienta especializada para detectar cualquier filtración de información sensible, como contraseñas, en nuestro repositorio de código. Esta medida es crucial para evitar la inadvertida exposición de datos confidenciales, lo que podría resultar en posibles vulnerabilidades o divulgación no autorizada de información.

### **Análisis de Dependencias (SBOM - Software Bill of Materials)**

Llevaremos a cabo un análisis completo de las dependencias de nuestro proyecto utilizando una herramienta especializada. Este análisis nos brinda un entendimiento profundo de las bibliotecas y componentes en los que confiamos, además de asistirnos en la identificación de posibles vulnerabilidades en estas dependencias. Esta etapa es esencial para garantizar la seguridad y estabilidad de nuestra aplicación a medida que evoluciona en su ciclo de vida.

### **Pruebas Unitarias e Integración**

Realizaremos pruebas unitarias para confirmar el adecuado rendimiento de las distintas secciones de nuestro código. Esta acción resulta fundamental para identificar y solucionar problemas o errores en una fase temprana, lo que contribuye a establecer la solidez de nuestra aplicación. Además, llevaremos a cabo pruebas de integración para asegurarnos de la coherente y eficiente interacción entre los diversos módulos y componentes en conjunto, garantizando un desempeño integral y confiable del sistema.

### **Análisis de Código Estático (SAST - Static Application Security Testing)**

Aplicaremos un análisis estático de seguridad en el código utilizando una herramienta especializada para buscar vulnerabilidades conocidas y problemas de calidad. La detección temprana de vulnerabilidades en las primeras etapas del proceso de desarrollo desempeña un papel fundamental en la prevención de posibles brechas de seguridad en el futuro. Esta evaluación minuciosa contribuye a garantizar la integridad y robustez del código a medida que se desarrolla y evita la propagación de problemas no detectados a etapas posteriores del proceso.

### **Análisis de Dockerfile**

En esta etapa, nos adentramos en la creación de imágenes de contenedor con un enfoque en la seguridad y la adhesión a las mejores prácticas. Para lograrlo, incorporamos un análisis riguroso de los Dockerfiles, lo que implica evaluar la estructura y el contenido en busca de posibles problemas o configuraciones que puedan comprometer la seguridad. Esta evaluación minuciosa asegura que nuestras imágenes de contenedor sigan pautas recomendadas, minimizando la exposición a vulnerabilidades y riesgos potenciales desde las primeras etapas del proceso de construcción.

### **Construcción de Contenedores**

La construcción de contenedores implica la creación de imágenes aisladas que encapsulan aplicaciones y sus dependencias en entornos portátiles. A través de archivos Dockerfile y mejores prácticas, se configuran entornos de ejecución seguros y eficientes. Durante este proceso, se automatiza la construcción, se verifica la integridad de componentes y se pueden aplicar firmas digitales para garantizar la autenticidad. Esta fase establece las bases para implementaciones coherentes y confiables en un entorno de producción.

### **Análisis de Contenedores**

Después de completar la construcción del contenedor, llevaremos a cabo un análisis exhaustivo para evaluar su seguridad. Durante este proceso, se examinarán minuciosamente los componentes del contenedor en busca de posibles vulnerabilidades y riesgos. La información obtenida a través de este análisis proporciona una visión detallada de la integridad y seguridad del contenedor, permitiéndonos tomar medidas proactivas para abordar cualquier posible punto de vulnerabilidad antes de implementarlo en el entorno de producción.

### **Firmado de Contenedores**

Con el objetivo de aumentar aún más la seguridad, aplicaremos medidas adicionales al firmar digitalmente nuestros contenedores utilizando Cosign. Las firmas digitales proporcionan verificación de autenticidad e integridad para los contenedores. Este paso asegura que los contenedores no hayan sido modificados y que provengan de una fuente confiable.

### **Análisis Dinámico (DAST - Dynamic Application Security Testing)**

En esta etapa crucial, realizaremos un análisis de seguridad dinámica mediante pruebas que simulan ataques en tiempo real sobre el código desplegado. Este proceso proporciona una perspectiva valiosa al identificar posibles vulnerabilidades y riesgos que podrían ser explotados por amenazas reales. Al explorar activamente las posibles debilidades de la aplicación durante su funcionamiento, esta fase nos permite tomar medidas preventivas para fortalecer aún más la resistencia y la seguridad de nuestra aplicación en un entorno de producción activo.

La implementación rigurosa de estas fases nos permite construir aplicaciones más seguras y confiables, al tiempo que reducimos los riesgos asociados con vulnerabilidades y brechas de seguridad. Cada paso contribuye de manera significativa a la creación de un proceso de desarrollo más robusto y orientado hacia la protección de nuestros sistemas y datos.
