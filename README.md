# Manual_De_Git
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
git git add .
```
Guardar los cambios del archivo en el sistema del control de versiones
```
git commit -m "[Mensaje del commot]"
```
