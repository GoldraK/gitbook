# Gitleaks

[GitLeaks (opens new window)](https://github.com/gitleaks/gitleaks)es una herramienta de seguridad utilizada en el ámbito de DevOps para detectar información confidencial y potencialmente comprometedora en repositorios de Git. Su objetivo principal es prevenir la filtración de datos sensibles, como contraseñas, claves de API y otros secretos, que podrían ser accidentalmente expuestos en el historial de versiones de un repositorio Git.

### [#](https://www-opensecdevops-6e927e11ce293189114b0f49928f13b830b2b5d21279a.gitlab.io/es/guide/gitleaks/#caracteristicas)Características <a href="#caracteristicas" id="caracteristicas"></a>

**Búsqueda de patrones sensibles:** GitLeaks busca patrones de datos sensibles utilizando reglas predefinidas o personalizadas. Estas reglas pueden incluir patrones de contraseñas, claves de API, tokens de autenticación y otros datos confidenciales.

**Análisis exhaustivo del historial:** La herramienta escanea el historial completo de commits en un repositorio Git, lo que incluye cambios antiguos y nuevos. Esto permite identificar y corregir datos sensibles que podrían haber sido agregados en versiones anteriores.

**Integración con flujos de trabajo de CI/CD:** GitLeaks se puede integrar en pipelines de CI/CD para realizar análisis de seguridad automáticamente antes de la implementación. Esto garantiza que cualquier nueva contribución sea examinada en busca de posibles fugas de información.

**Compatibilidad con múltiples formatos de archivos:** GitLeaks es capaz de analizar varios formatos de archivos, como archivos de código fuente, archivos de configuración y archivos de texto plano. Esto abarca una amplia gama de posibles ubicaciones de datos sensibles.

**Configuración personalizada:** Los usuarios pueden configurar las reglas y los patrones de búsqueda según las necesidades específicas de su proyecto, lo que permite adaptar GitLeaks a diferentes contextos.
