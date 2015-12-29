# Git

* Se sigue el esquema de rama 'master' y 'develop' en el repositorio de github, donde la rama 'master' debería tener todo codigo testeado listo que siempre estaría listo para producción, y la rama 'develop' para desarrollo. Pueden surgir branch de otras ramas, pero siempre de la rama 'develop' y por lo general son ramas locales
* Escribir commit en español
* Se comienza siempre con la primera letra en mayuscula. Ejemplo: Primer commit
* No finalizar frase con punto
* Hablar en presente y no en pasado. Ejemplo: Renombra nombre de usuario. Corrige error al intentar logearse con rut invalido
* Evitar palabras como 'se'. Ejemplo malo: Se Corrige. Ejemplo bueno: Corrige
* Referirse siempre sobre la nueva funcionalidad del codigo
* Idealmente primera linea (Sujeto) 50 caracteres máximo, y en modo imperativo, como si se tratara de una orden. Ejemplo: Actualiza la documentacion inicial. Remueve metodos deprecados. Refactoriza funcion X
* Utilizar un cuerpo o descripción en caso que se requiera. Debe ir separada por un salto de linea del sujeto. Ejemplo:

```
Resume cambios en 50 caracteres o menos

Este es el texto explicativo, en caso que sea necesario.
Comienza tambien con la primera letra en mayuscula y separada
por un salto de linea del sujeto. La linea de separacion es critica
para herramientas como `log`.
```

Basado en [How to write a Git Commit Message](http://chris.beams.io/posts/git-commit/)
