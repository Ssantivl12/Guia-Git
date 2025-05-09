# ¿Qué hace Git Merge?
Como ya vimos, `git merge` se usa para fusionar los cambios de una rama con otra, siendo útil cuando trabajaste en una rama nueva *nueva-funcionalidad* y ahora quieres que esos cambios que integren en la rama *main*, para ello debes estar en la rama *main* y recien realzar el comando `git merge nueva-funcionalidad` para traer los cambios a la rama </br>

Pero debemos tener cuidado al realizar estas fusiones porque pueden ocasionares conflictos

## ¿Por qué ocuren los conflictos?
Los conflictos ocurren cuando Git no sabe como combinar los cambios de ambas ramas, esto puede pasar cuando

- Dos ramas tienen los cambios en una misma línea de un archivo
- Un archivo fue eliminado en una rama y modificado en otra  

Por ello Git no puede adivinar cual cambio es correcto y te solicitará resolverlo


