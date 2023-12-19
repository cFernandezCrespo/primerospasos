# examenSRI
## Parte 1
### Realiza una imagen personalizada de Alpine en la que se pueda utilizar un navegador de terminal

### 1) Escribe el Dockerfile

Comenzaremos creando el docker file para tener nuestra version de alpine modificada para trabajar para nosotros, en la imagen siguiente podreis ver lo que fui añadiendo, la ultima versión de alpine, varias herramientas utiles para utilizar dentro de la misma como herramientas de dns y demás y por ultimo añadí la forma de hacer que se añada el navegador para lanzar comandos.

![imagen primera parte](imagenes/Screenshot_20231121_163847.png)

### 2) Sube la imagen al docker hub

En las siguientes imagenes enseño como subirlo a dockerhub

### 3) Pon en el Readme el enlace a la imagen en el docker hub

Aquí tienes 
~~~
https://hub.docker.com/repository/docker/carlosferncres/examensri/general
~~~

## Parte 2 

### Apache virtual host 

### 1)Crea un contenedor apache con dos virtual host que se distingan por el puerto

### 2)Comprueba con el contenedor de alpine que accedes a dos páginas diferentes en distintos puertos

### 3)Todo está integrado en un docker compose