---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Finding

Los "finding" en DefectDojo son registros que representan hallazgos o descubrimientos de problemas de seguridad en una aplicación o proyecto. Estos problemas pueden incluir vulnerabilidades de código, debilidades en la configuración, errores de seguridad y otros riesgos relacionados con la seguridad.

Generalmente se crean como parte del proceso de análisis de seguridad de una aplicación. Los profesionales de seguridad, ingenieros de pruebas y desarrolladores pueden identificar estos problemas durante la ejecución de pruebas de seguridad, análisis estático de código, análisis dinámico de aplicaciones, escaneo de contenedores, revisión de configuraciones y otras actividades relacionadas con la seguridad.

Cada "finding" en DefectDojo suele contener información detallada sobre el problema:

1. **Descripción Detallada**: Cada "finding" incluye una descripción detallada del problema de seguridad. Esta descripción proporciona información precisa sobre el problema, lo que facilita su comprensión y abordaje por parte del equipo de desarrollo y seguridad.
2. **Gravedad**: Los "finding" se clasifican por gravedad para indicar su impacto potencial en la seguridad. Esta clasificación ayuda a priorizar la corrección de problemas, asegurándose de que los más críticos se aborden primero.
3. **Tipo de Vulnerabilidad**: Se asocia un tipo de vulnerabilidad específico a cada "finding". Esto ayuda a identificar la naturaleza del problema de seguridad, como inyecciones SQL, vulnerabilidades de seguridad de la capa de transporte (TLS/SSL), ataques de denegación de servicio (DoS), entre otros.
4. **Ubicación**: Los "finding" incluyen información sobre dónde se encuentra el problema. Esto puede incluir referencias al código fuente, a archivos específicos, a URL o endpoints en aplicaciones web, o incluso a configuraciones específicas de infraestructura.
5. **Evidencia y Contexto**: Para comprender mejor el "finding", se pueden adjuntar evidencias o pruebas relacionadas. Esto puede incluir fragmentos de código, capturas de pantalla, registros o cualquier otra información que respalde el hallazgo. Además, se proporciona contexto para ayudar a los equipos a entender el alcance y el impacto del problema.
6. **Asignación de Responsabilidad**: Cada "finding" se puede asignar a un miembro del equipo responsable de corregirlo. Esto asegura que haya un propietario claro para cada problema de seguridad.
7. **Estado y Progreso**: Los "finding" pueden tener estados que indican si están pendientes, en progreso o resueltos. Esto permite realizar un seguimiento del progreso de la corrección y garantizar que se resuelvan los problemas.
8. **Historial y Auditoría**: Se realiza un seguimiento completo de cambios y actualizaciones en cada "finding", lo que proporciona un historial completo de actividades y una auditoría de quién hizo qué y cuándo.
9. **Comentarios y Discusión**: Los "finding" permiten comentarios y discusiones entre miembros del equipo de desarrollo y seguridad, lo que facilita la comunicación y colaboración en la resolución de problemas.
10. **Priorización y Planificación**: Los "finding" se pueden priorizar para abordar los problemas más críticos primero. Esto ayuda en la planificación de acciones de corrección y asignación de recursos.
