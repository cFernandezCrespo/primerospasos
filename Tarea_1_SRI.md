# Tarea 1
## Descarga la imagen 'ubuntu y comprueba que está en tu equipo
docker run -it ubuntu:latest bash
<br/><br/>
Realmente este comando te arranca una máquina instalando si no lo tuvieras por el camino esa imagen de ubuntu pero realmente sirve de la misma forma

docker images<br/><br/>
Con este comando puedes conocer mucha de la información importante de las imágenes de docker como cuanto pesan o cuantas tienes

## Crea un contenedor sin ponerle nombre. ¿está arrancado? Obtén el nombre
docker run -it ubuntu:latest bash<br/><br/>
Nos sirve el mismo comando de antes porque realmente vale para esto, de esta forma el docker nos dará un nombre aleatorio predeterminado.
docker ps
Con este comando puedes ver las máquinas que están arrancadas y ver que la que acabamos de crear efectivamente está arrancada.

Crea un contenedor con el nombre 'ubu1'. ¿Como puedes acceder a él?
docker run -it --name ubu1 ubuntu bash
Con solo una línea de comando la creamos y al mismo tiempo accedemos a él.

## Comprueba que ip tiene y si puedes hacer un ping a google.com
haces ipconfig y te das cuenta de que no tiene ip porque no tiene net tools haces apt update y luego apt install net-tools, luego apt install iputils-ping para poder hacer ping y ahora con ifconfig deberías ver la ip y con ping a 8.8.8.8 te deberia salir<br/>
## Crea un contenedor con el nombre 'ubu2'. ¿Puedes hacer ping entre los contenedores?
docker run -it --name ubu2 ubuntu bash<br/>
Creamos el contenedor y al igual que antes tienes que hacer actualizar, nettools y el
iputils, ahora con ello hecho con ifconfig vemos la ip de ambos y en cualquiera de
los dos deberíamos poder hacer ping (ip destino) y debería funcionar.

## Sal del terminal, ¿que ocurrió con el contenedor?
se cierra de forma automática, tendríamos que arrancar el contenedor de nuevo<br/>
## ¿Cuanta memoria en el disco duro ocupaste? ¿Hay alguna herramienta de docker para calcularlo?
puedes ver el tamaño de las images y los contenedores por separado con el comando docker system df con eso te aparece toda la información que necesitas.

## ¿Cuanta RAM ocupan los contenedores? Crea cuántos contenedores necesites para calcularlo.
Pues utilizando docker stats puedes ver cuánto consumen tus contenedores activos y ahora mismo cada uno gasta entre 800 y 900 KiB de memoria RAM
