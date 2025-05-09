# Conventional commits y buens prácticas

## Conventional commits

Los conventional commits son una convención para nombrar los mensajes del commit de manera consistente y comprensible, mayormente útil en proyectos colaborativos, donde la estructura es </br>

<tipo [alcance, opcional]>: descripción corta

Los tipos comunes son:

- feat: nueva funcionalidad

- fix: corrección de errores

- docs: cambios en la documentación

- style: cambios de formato (espacios, comas, etc.)

- refactor: cambios en el código que no agregan ni corrigen funcionalidades

- test: agregar o modificar tests

- chore: tareas internas (como actualizar paquetes)

## Buenas prácticas 

Las buenas prácticas para realizar los commits serían las siguientes:

- Escribe mensajes claros, por ejemplo "fix: corrección validación del correo" 

- Commits pequeños y específicos, no mezclar cosas no relacionadas

- Usa `git status` o `git diff` antes de hacer commit, para estar seguro de lo que vas a guardar

## Definición de rango de cambios para los commits

La regla general indica que para un commit efectivo debe representar una unidad lógica **completa** de trabajo

### Pautas oara decidir que incluir en un commit

- Unidad atómica de trabajo: Un commit debe representar un cambio completo y funcional. Si divides demasiado tus commits, podrías dejar el código en un estado no funcional

- Propósito único: Cada commit debe tener un propósito claro y único. Por ejemplo, "implementar modelo X" o "corregir error en Y"

- Facilidad de revisión: Un buen commit debe ser fácil de revisar. Si tiene demasiados cambios no relacionados, dificultará la revisión

- Tamaño razonable: Aunque no hay un límite estricto, un commit no debería tener cientos de archivos modificados (a menos que sea algo como un cambio de formato automático)

# Trucos de Git

-  `git reset --soft HEAD~1` Deshacer el último commit sin perder los cambios (Vuelve tu último commit al staging area, útil si olvidaste agregar algo o quieres cambiar el mensaje)

Los alias te permiten abreviar comandos largos o que usas con mucha frecuencia </br>

`git config --global alias.<alias> '<comando completo>'` </br>

Aplicado a un comando muy utilizado `git config --global alias.loda 'git log --all --oneline --decorate'`

