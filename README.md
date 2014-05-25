mailTemplate
============

Herramienta para crear templates para mensajes de correo electrónico.

Aqui un cambio realizado por alephart usuario.

----------------------------------
Cambios por arjc
----------------------------------
Aqui se agregan mas lineas. Esto se pudo gracias a que primero se realizo la descarga del original en remote y se psa a editar, inicialment en otra rama para despues mezclar:

$ git pull origin master
$ git checkout -b master-pre-merge
$ git merge desarrollo

Ahora a modificar archivos y despues a terminar haciendo el pull request

----------------------------------
Escrito por valore
----------------------------------
Despues que arjc realizo cambios tuve que bajar o actualizar en mi local el remoto:
$ git pull origin master

Tenia unos ajustes en el master y habia creado un archivo nuevo, de modo que no me permitio la escarga y me informo que debia ajustar el commit o desaserlo.

Hice una copia en otra Rama y pase a eliminar los ajustes en Master:

$git checkout -b mi-rama-prueba

Agregue los archivos que estaban pendientes:

$git add README.md

Ahora hice el commit:

$git commit -m "notas de mi ajuste en nueva rama"

Ahora cambio a la rama Master  y dejo el HEAD como estaba antes de mis cambios:

$git reset --hard

Ahora si el pull:

$git pull origin master

Con el repositorio original aqui procedo a realizar mis cambios. Los de la otra rama ya son otros cambios, hice una copia pero sera solo eso, una copia.

Ahora procedo a subir mis cambios:

$git push origin master
----------------------------

Hay muchas dudas, pero igual las ire dilusidando a medida que vamos aprendiendo con git, por ejemplo:

- Que Workflow utilizar segun el tipo de proyecto y colaboradores.
- Como modificar contenido de varias ramas sin necesariamente el editor definido en linea de comandos.
- Si utilizo Sublime Text??? bueno voy a buscar un pluggin para git... 

RECORDAR:

Despues de un cambio se debe:

- agregar el archivo modificado en la rama donde se este:
$git add archivo

- hacer el commit
$git commit -m "descripcion"

- subir la rama o hacer merge a la rama Master (si no se esta en Master)
$git push origin la-rama 
$git push la-rama-remote la-rama-local

Listo!








