# Introducción a Git
Git es una herramienta de control de versiones, que registra los cambios en los archivos, permitiendo comparar los versiones, ver el historial de cambios y revertir a estados anteriores. Además es distribuido, lo que quiere decir que; cada desarrollador tiene su propia copia del repositorio, facilitando la colaboración entre equipos permitiendo que diferentes desarrolladores trabajen en un mismo proyecto a la vez de manera coordinada y ordenada

## Instalación de Git
<details>
<Summary> Paso a paso </Summary>

La descarga se debe realizar desde la página oficial de [Git](https://git-scm.com/downloads) y elige la versión dependiendo de tu sistema operativo </br>
Luego de descargar, ejecuta el archivo y comenzamos con la instalación </br>

1. Como primer paso debemos leer y aceptar la licencia 
<div align="center">
  <img src="assets/images/introduccion/1-int.jpg" alt="Captura" width="40%"/>
</div>

2. Elegimos el directorio en el que será instalado (recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/2-int.jpg" alt="Captura" width="40%"/>
</div>

3. Instalación de componentes (recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/3-int.jpg" alt="Captura" width="40%"/>
</div>

4. Elegit el editor de texto para Git (recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/4-int.jpg" alt="Captura" width="40%"/>
</div>

5. Selecciona el nombre de la rama inicial (por defecto es ‘master’, pero puedes cambiarlo a ‘main’ al crear un nuevo repositorio)
<div align="center">
  <img src="assets/images/introduccion/5-int.jpg" alt="Captura" width="40%"/>
</div>

6. Ajustar el entorno de ejecución de Git (recomendado dejar el valor predetermminado, permitiendo ejecutar Git desde otras terminales de comando)
<div align="center">
  <img src="assets/images/introduccion/6-int.jpg" alt="Captura" width="40%"/>
</div>

7. Elegir la Shell que usará Git (recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/7-int.jpg" alt="Captura" width="40%"/>
</div>

8. Elección del backend de transporte HTTPS (recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/8-int.jpg" alt="Captura" width="40%"/>
</div>

9. Cada sistema operativo tiene una manera diferente de representar los finales de linea (CRLF y LF), se recomienda dejar marcada la opción por defecto para asegurar que no haya errores por diferencias de formatos entre sistemas operativos
<div align="center">
  <img src="assets/images/introduccion/9-int.jpg" alt="Captura" width="40%"/>
</div>

10. Elegir el emulador de terminal para Git Bash(recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/10-int.jpg" alt="Captura" width="40%"/>
</div>

11. Elegir el comportamiento de Git cuando se realice un 'pull' (recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/11-int.jpg" alt="Captura" width="40%"/>
</div>

12. Elegir el manejador de credenciales (recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/12-int.jpg" alt="Captura" width="40%"/>
</div>

13. Configuraciones extra (recomendado dejar el valor predetermminado)
<div align="center">
  <img src="assets/images/introduccion/13-int.jpg" alt="Captura" width="40%"/>
</div>

14. Configurar opciones experimentales (No marques ninguna casilla a menos que sepas exactamente qué hacen y por qué las necesitas)
<div align="center">
  <img src="assets/images/introduccion/14-int.jpg" alt="Captura" width="40%"/>
</div>

15. Continuando se instalará Git con las opciones elegidas
<div align="center">
  <img src="assets/images/introduccion/15-int.jpg" alt="Captura" width="40%"/>
</div>

16. Terminada la instalación se mostrará un panel indicando que la instalación ha sido completada correctamente
<div align="center">
  <img src="assets/images/introduccion/16-int.jpg" alt="Captura" width="40%"/>
</div>

17. Por último se debe corroborar la instalación abriendo una nueva terminal (CMD o PowerShell en el caso de Windows) y ejecutando el comando `git --version` , mostrando la versión de Git que se instaló
<div align="center">
  <img src="assets/images/introduccion/17-int.jpg" alt="Captura" width="40%"/>
</div>
</details>


## Primeros comandos

Ya instalado correctamente Git comenzaremos con la explicación de una serie de comandos principales

- `git init` : Primer comando que se debe realizar al iniciar un proyecto, inicializa Git crea un repositorio local
- Configura tu identidad, antes de hacer tus primero commits debes indicarle Git quien eres, esto para que pueda registrar correctamente tus cambios en el historial
    + `git config --global user.name "Tu Nombre"`
    + `git config --global user.email "tuemail@example.com"`
    El uso de `--global` indica que esa configuración a todos los proyectos de tu computadora

- `git add ` Añade archivos al [staging area](#staging-area). Se puede usar `git add .` para añadir todos los archivos con cambios o `git add archivo.txt` para añadirlos uno por uno
- `git commit` [Guarda los cambios agregados al staging area](#guardado-de-cambios-commits),este te solicitará un mensaje para nombrar los cambios a guardar, tambien se puede usar `git commit -m "mensaje"` para ingresar el mensaje en un solo comando 
- `git status` Muestra el estado de los archivos, si fueron o no agregados al staging area
- `git log` Muestra el historial de los commits ya realizados, incluye la fecha, mensaje y el autor de cada uno
<div align="center">
  <img src="assets/images/comandos-conceptos-basicos/git-log.jpg" alt="Captura" width="40%"/>
</div>
</details>

## Conceptos básicos 

### Staging area
Es una *zona intermedia* en la que estan los archivos que estan listos para ser guardados. Es una lista de cambios que le diras a Git que quieres conservar, solo los archivos en el staging area se incluiran en el siguiente commit

### Guardado de cambios (Commits)
Un commit es como una foto del estado actual de tu proyecto. Cada commit guarda los cambios realizados, permitiendo volver a estados anteriores si algo sale mal y conforman el historial de desarrollo 

