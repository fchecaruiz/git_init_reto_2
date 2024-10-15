- Primero instalar Git en el pc
- Una vez que este instalado, creamos un repositorio nuevo en git hub
- New => Clikeamos en new para nuevo repositorio
- Añaimos nombre de repositorio y denajo, una descripcion opcional
- Clikemaos en PUBLIC o PRIVATE (depende de nosotros mismos)
- Add readme.md, opcional
- Creamos repositorio

# AHORA NOS VAMOS AL PC
- Clonamos el repositorio que hemos creado recientemente
- Abrimos Terminal
- Vamos a git hub, y en la esquina superio derecha click en <>CODE 
- Copiamos la URL que tenemos 
- Nos vamos a la terminal y escribimos:
git clone "direccion de la URL copiada en github" + enter
- Escribimos:
git status para ver el estado del repositoro.Verificamos el estado actual de los archivos.
- Modificamos el archivo, lo trabajamos.....etc. Una vez modificado escribimos en la terminal.
git add . + enter (Aqui se añade toda la modificaion de los archivos que hayamos trabajado con ellos).
Este punto seria el STAGE
- de nuevo para comprobar:
git status + enter
- Ahora hacemos un COMMIT , que este actualiza los ficheros a la modificaion actual y siempre el LOCAL
git commit -m "nombre de la actualizacion que hemos hecho o explicamos que hemos modificado".
En caso de poner git commit y darle al ENTER sin poner la -m, la terminal se bloquea y hay que desbloquear la terminal de la siguiente manera:
Pulsa ESC , q,! + ENTER
- Una vez hecho el commit, y tenemos los archivos en local, si queremos pasarlos a la nube, a git hub, tendremos 
que añadir :
git push (CON GIT PUSH LOS ARCHIVOS PASAN A REMOTO).
Una vez hecho el push, vamos a github , refrescamos la pagina y nos deberia salir el repositorio con los archivos modificados por nuestra parte.
- Tambien tenemos la opcion inversa a git push, que es git pull:
git pull => Trae archivos del repositorio de git hub al pc, es decir, pasa los archivos de remoto a local
- Cuando queremos trabajar en un proyecto conjunto, deberemos abrir una rama para nuestro trabajo interno, y asi, 
poder trabajar y no molestar ni que nos molesten en nuestro trabajo del dia a dia.
Para generar una rama se hace de la siguiente forma:
git branch nombre de la rama que queramos poner.
En caso de abrir una o mas ramas, podemos hacerlo hacerlo sin ningun problema.
- Una vez que estamos trabajando, para saber en que rama estamos,o para cambio de rama se hace con el checkout :
git checkout + enter
gir checkout nombre de rama que queramos entrar .
- Una vez terminado el trabajo en la rama, es hora de fusionarlo con la rama principal o rama main :
git merge nombre de la rama + enter(fusiona la rama con la main).
- y por el ultimo, cuando trabajamos con mucos archivos y lo svamos modificando, hay siempre algunos archivos
que no queremos enviar a git hub y los queremos guardar en local. Para esto hay que abrir una carpeta (aconsejable antes de haer el STAGE) CON GIT IGNORE y ahi meter los archivos de forma manual, indicando el nombre de los archivos que queremos reservar para nosotros 
git ignore + enter 
