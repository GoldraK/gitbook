# Engagement

En DefectDojo, un "engagement" se refiere a un proyecto específico o una actividad que implica la identificación y mitigación de vulnerabilidades en una aplicación o sistema. Los engagements son una parte fundamental de la gestión de la seguridad en DefectDojo, ya que te permiten llevar un registro de las pruebas de seguridad, auditorías y evaluaciones que se realizan en tus productos o aplicaciones.

Cada engagement puede representar una variedad de actividades, como:

1. **Pruebas de Penetración**: Cuando un equipo de seguridad o un auditor externo intenta identificar vulnerabilidades en una aplicación mediante ataques controlados.
2. **Evaluaciones de Aplicaciones**: Evaluaciones sistemáticas de una aplicación para identificar posibles riesgos de seguridad.
3. **Auditorías de Código**: Revisiones del código fuente en busca de vulnerabilidades y problemas de seguridad.
4. **Análisis de Escaneo de Vulnerabilidades**: Escaneos automáticos de vulnerabilidades que identifican riesgos en una aplicación o sistema.
5. **Pruebas de Seguridad Continuas**: Pruebas regulares y automatizadas que se ejecutan durante todo el ciclo de vida del desarrollo.
6. **Pruebas de Cumplimiento**: Evaluaciones que garantizan que una aplicación cumpla con los estándares de seguridad y regulaciones específicas.
7. **Evaluaciones de Terceros**: Auditorías realizadas por partes externas, como empresas de seguridad independientes.

### Tipos de Engagement

En DefectDojo, tenemos dos tipos de engagement los "Interactive Engagements" como los "CI/CD Engagements" son tipos específicos de compromisos utilizados para organizar y gestionar las actividades relacionadas con la seguridad en una aplicación o proyecto. Sin embargo, tienen diferencias clave en cuanto a su naturaleza y propósito:

**Interactive Engagement (Compromiso Interactivo)**:

* **Naturaleza Interactiva**: Estos compromisos implican interacción activa de un equipo de seguridad, auditor o profesional de seguridad con la aplicación o sistema. En otras palabras, se trata de pruebas de seguridad que requieren la intervención manual y la toma de decisiones por parte de expertos en seguridad.
* **Pruebas de Penetración**: Los Interactive Engagements suelen relacionarse con pruebas de penetración o evaluaciones de seguridad manuales. Implican la búsqueda activa de vulnerabilidades, explotación de posibles debilidades y un análisis en profundidad de la seguridad de la aplicación.
* **Escenario Realista**: Estos compromisos suelen replicar escenarios de ataque realistas para evaluar la capacidad de la aplicación para resistir intentos de explotación y para identificar posibles riesgos de seguridad.

**CI/CD Engagement (Compromiso CI/CD)**:

* **Automatización y Continuidad**: Los CI/CD Engagements están más relacionados con las pruebas automatizadas y continuas de seguridad que se integran en el flujo de trabajo de desarrollo (CI/CD). Son parte de un proceso de desarrollo ágil y se ejecutan de manera regular, incluso después de la implementación de cambios.
* **Enfoque en la Integración y Entrega Continua (CI/CD)**: Estos compromisos se centran en evaluar la seguridad durante todo el ciclo de vida del desarrollo, especialmente en entornos CI/CD. Se utilizan para garantizar que las nuevas actualizaciones y características no introduzcan vulnerabilidades en la aplicación.
* **Automatización de Pruebas de Seguridad**: Los CI/CD Engagements suelen incluir escaneos automáticos de seguridad, análisis de código estático y dinámico, escaneos de vulnerabilidades de contenedores y otras pruebas automatizadas.

En resumen, la principal diferencia radica en la naturaleza de las actividades de seguridad que abordan. Los Interactive Engagements se centran en pruebas manuales y actividades de penetración que requieren interacción humana activa, mientras que los CI/CD Engagements se centran en pruebas automatizadas y continuas que se integran en el proceso de desarrollo para garantizar la seguridad en todo momento. Ambos tipos de compromisos son esenciales para una estrategia de seguridad completa en una organización.

### Creación

Para aquellos que lo integremos con el CI de GitLab, crearemos un engagement del tipo CI/CD cada vez que se ejecute nuestro pipeline. Esto nos permitirá separar las pruebas de commit en su propio grupo de pruebas. Si el equipo de desarrollo es grande y se generan muchos pipelines, esto podría implicar un mayor trabajo para los equipos de SecDevOps. Sin embargo, nos proporcionará una mayor claridad sobre qué commit y qué usuario ha cometido prácticas deficientes, lo que nos permitirá abordarlas y evitarlas en el futuro de manera más efectiva.\
Para ello vamos a crear un stage previo en el CI que podemos ver en la sección de Integraciones Monitorización
