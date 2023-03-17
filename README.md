# Manual de Git y Github
Este es un pequeño manual de los comandos más usado en el sistema de control de versiones de git

## ¿Qué es un repositorio en git?
Un repositorio de Git es un almacenamiento virtual de tu proyecto. Te permite guardar versiones del código a las que puedes acceder cuando lo necesites.

## ¿Dónde se puede descargar git?
para descargar git, se debe de ingresar a la pagina principal [Git](https://git-scm.com/) Una vez dentro se debe de buscar en el apartado en de descarga

## ¿Qué sistema usas?
Dependiendo del sistema se debe de instalar de diferente forma, en el caso de windows, solamente se debe de descargar el .exe y ejecutar como administrador, se deben de aceptar en toda las ventanas emergentes que salga a la hora de instalación.
En el caso de linux si es derivado de debian se debe de ejecutar el siguiente comando:
```
sudo apt install git
```
Para ver si se instalo git y su version, ejecutar:
```
git --version
```
## Configuración inicial 
Una vez que se instaló git se debe de configurar. En este caso se debe de configurar el correo y el nombre del usuario, esto se hace para saber que usuario hizo registro y para poder subir el código a un repositorio remoto.
La configuración del nombre:
```
git config --global user.name "[Mi nombre]"
```
La configuración del correo:
```
git config --global user.email "[Mi email]"
```
Para ver la configuracion 
```
git config --list
```
## Iniciando el proyecto
Para iniciar un repositorio en el directorio actual
```
git init
```
Si se buscar ver el estado del repostorio
```
git status
```
Guardar el estado del archivo
```
git add "[nombre del archivo]"
```
Para guardar e incluir todo los archivo del repositorio
```
git add .
```
Fechero especial para excluir archivos, extension, ruta
```
.gitignore
```
Guardar los cambios del archivo en el sistema del control de versiones
```
git commit -m "[Mensaje del commit]"
```
Comando para cambiar entre ramas y commit, ademas sirve para regresar del area de trabajo
```
git checkout "opcion"
```
Para borrar el archivo y situarlo en el estado de eliminacion
```
git rm
```
Muestra el estado del repositorio
```
git log
```
Crear un alias personalizado para poder abreviar otro mas complejo
```
git alias
```
Muestra las diferencias entre achivos
```
git diff
```
Situar el archivo en el area de espera manteniendo su contenido
```
git reset
```
Muestra toda las referencia asociadas al commits del proyecto 
```
git reflog
```
Asocia una etiqueta a un commit
```
git tag
```
## Trabajando con Ramas 
Tip como buenas practicas 
1. ![Trabajo en equipo](https://github.com/JoseLeviRivera/Manual_De_Git/blob/main/trabajo%20en%20equipo.jpeg)
1. ![A la hora de trabajar con ramas](https://raw.githubusercontent.com/JoseLeviRivera/Manual_De_Git/main/ramas.webp)
### Comandos para trabajar con ramas
Para crear una rama 
```
git branch
```
Otra opcion para crear una rama y desplazarse a la misma rama creada
```
git checkout -b "[nombre de la rama]"
```
Permite cambiar entre ramas
```
git switch
```
Combinar el historial de commits con otra rama diferente a la actual
```
git merge
```
Almacena cambios temporales, los recupera, lista y elimina
```
git stash [pop|list| drop]
```
Especifica el directorio remoto donde se aloja el proyecto de git 
```
git remote
```
Para descargar un repositorio
```
git clone
```
Descargar el historial sin incorporar los cambios 
```
git fetch
```
Descargar el historial incorporando los cambios 
```
git pull
```
Sube los cambios a la rama
```
git push
```
Permite añadir commits concretos de otras ramas a tu rama
```
git cherry-pick
```
integra modificaciones de una rama en otra y actualiza el historial
```
git rebase
```
Muestra los datos del commit especifico
```
git show[commit]
```
Cambia el nombre del archivo y lo prepara para su guardado
