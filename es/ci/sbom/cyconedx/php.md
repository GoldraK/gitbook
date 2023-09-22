# PHP

Para instalar [CycloneDX en PHP con Composer](https://github.com/CycloneDX/cyclonedx-php-composer), primero debes asegurarte de que tengas PHP y [Composer](https://getcomposer.org/) instalados en tu sistema. Luego, sigue estos pasos:

* Abre una terminal o línea de comandos.
* Navega hasta la raíz de tu proyecto PHP, donde se encuentra tu archivo `composer.json`.
* Ejecuta el siguiente comando para agregar CycloneDX como una dependencia de desarrollo:

```bash
composer require --dev cyclonedx/cyclonedx-php-composer
```

* Permitimos el plugin de CycloneDX, para eso tenemos que agregar al `composer.json`  lo siguiente

```json
    "config": {
        "allow-plugins": {
            "cyclonedx/cyclonedx-php-composer": true
        }
    }
```

* Ya  podemos ejecutar el análisis de dependencias mediante CycloneXD con el siguiente comando

```bash
composer CycloneDX:make-sbom --output-file=sbom.json --output-format=json
```

