# Desarrollo

En el proceso de desarrollo de software, es esencial adoptar buenas prácticas que aseguren la consistencia, la seguridad y la colaboración efectiva entre los miembros del equipo. Una de las formas más eficientes de lograr esto es a través del uso de contenedores y la implementación de medidas de seguridad robustas. Para ello en el marco de trabajo se propone algunas prácticas:

### **Contenedores estandarizados y firmados**

En un entorno de desarrollo colaborativo, es crucial que todos los miembros del equipo trabajen en un entorno homogéneo y predecible. Aquí es donde entran en juego los contenedores. Estos entornos autocontenidos encapsulan todas las dependencias, configuraciones y herramientas necesarias para ejecutar una aplicación de manera consistente, independientemente del sistema operativo del desarrollador. Al adoptar una arquitectura basada en contenedores, todos los programadores pueden crear, modificar y compartir las mismas configuraciones de manera sencilla, lo que reduce la variabilidad en los entornos de desarrollo y elimina problemas relacionados con diferencias en configuraciones locales.

Además, al firmar digitalmente los contenedores, se agrega una capa adicional de seguridad y autenticidad. Esto garantiza que las imágenes utilizadas estén libres de manipulación malintencionada y provengan de una fuente confiable. Los contenedores firmados son una práctica segura y confiable para asegurarnos de que las imágenes que utilizamos sean genuinas y seguras.

Dichos contenedores tienen que crearse en coordinación entre los desarrolladores y el equipo de SecDevOps tanto para que sean útiles como para que se mantengan actualizados y seguros.

### **Gestión de Código**

La gestión del código en repositorios Git también juega un papel crucial. Conectar a estos repositorios mediante claves SSH en lugar de contraseñas tradicionales mejora la seguridad al eliminar la exposición accidental de credenciales y fortalecer la autenticación. Esto se traduce en una mayor protección de los datos sensibles y contribuye a la confianza en la integridad del proceso de desarrollo.

### Estándares de desarrollo

Es fundamental que los programadores sigan los estándares y marcos de desarrollo establecidos para cada lenguaje. Estos marcos de trabajo, como el PSR (PHP Standards Recommendations) para PHP o los PEP (Python Enhancement Proposals) para Python, son guías detalladas que establecen convenciones y mejores prácticas para escribir código limpio, legible y coherente.

Seguir estos marcos de desarrollo no solo mejora la consistencia en el código, sino que también facilita la colaboración en equipos y la mantenibilidad a lo largo del tiempo. Estos estándares abordan aspectos como la nomenclatura de variables, la estructura del código, el formato de las tabulaciones y otros detalles que pueden afectar la calidad y la legibilidad del código.

Al adherirse a los estándares y marcos de desarrollo específicos de cada lenguaje, los programadores contribuyen a un entorno de desarrollo más unificado y eficiente. Esto permite que el equipo trabaje de manera armoniosa, evitando confusiones y reduciendo la posibilidad de errores derivados de diferentes enfoques de codificación. En última instancia, esta práctica fortalece la calidad del código y la consistencia en todo el proyecto, brindando una base sólida para el éxito a largo plazo.
