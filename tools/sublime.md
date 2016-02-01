# Sublime

* Usar Package Control para gestion de plugin

# Packages

* [Editor Config](https://github.com/sindresorhus/editorconfig-sublime): Para la consistencia y estandarizacion del estilo del codigo para cada lenguaje de programación, el cual es usado en el proyecto base de laravel

* [SublimeLinter](http://www.sublimelinter.com/en/latest): Para detectar

## SublimeLinter-php y SublimeLinter-phpcs

* Requerimiento tener instalado php y [phpcs](https://github.com/squizlabs/PHP_CodeSniffer)

Para chequear el codigo que no presente errores de sintaxis, y que siga el estandar PSR-2 se debe instalar 'SublimeLinter-php' y 'SublimeLinter-phpcs'. Luego configurarlo de la siguiente forma:

```
Preferences -> Package Settings -> SublimeLinter -> Settings - User menu item
```

```json
{
    "user": {
        "delay": 0.5,
        "linters": {
            "php": {
                "@disable": false,
                "args": [],
                "excludes": []
            },
            "phpcs": {
                "@disable": false,
                "args": [
                    "-n"
                ],
                "excludes": [
                    "*Test.php"
                ],
                "standard": "PSR2"
            }
        },
        "paths": {
            "osx": [
                "${directory}/vendor/bin/",
                "${project}/vendor/bin/",
            ],
            "linux": [
            ],
            "windows": [
            ]
        }
    }
}
```

<img src="/assets/sublimelinter-psr2.png"/>

## SublimeLinter-jscs y SublimeLinter-jshint

* Requerimiento tener instalado node, jshint, jscs

* https://packagecontrol.io/packages/SublimeLinter-jscs
* https://github.com/SublimeLinter/SublimeLinter-jshint



