
Hola Siempre Listos

GIT ALL <NOMBRE DE ARCHIVO>: Escribir el comando git add <archivo> para agregar los cambios de un archivo especifo al staging

git diff hash archivo: compara el archivo actual con el archivo referenciado con el hash
git add: Sirve para agregar todos los cambios realizados en el directorio  donde uno se encuentra al staging.
git add . : ara agregar todos los archivos del directorio actual.


git revert <ID del commit>  esto creara un nuevo commit que deshace los cambios realizados en el commit anterior .

git branch: enumera tus sucursales. Aparecerá un * junto a la rama actualmente activa.

git Checkout <Nombre de la rama> Poder llegar hasta el id de la rama que se coloque.

git init: inicializara un repositorio git en la direccion actual.




git reset: te permite deshacer cambios sin crear un nuevo commit a diferencia del revert que solo se puede en local 
este se puede ver en servidor

git push: con este comando podemos subir al repositorio remoto en el que estamos trabajando, siempre y cuando lo hayamos clonado inicialmente.

git commit -m "mensaje": captura una instantánea de los cambios preparados en ese momento del proyecto .

git commit --amend: Se utiliza para modificar el ultimo commit, te permite añadir archivos o cambiar el texto del commit
### Git Diff
Escribir el comando git diff <archivo> y presionar enter. Esto mostrará las diferencias del archivo.

git status: Sirve para mostrar el estado del repositorio, para identificar archivos modificados y en general para estar informado sobre el estado actual del repositorio

git merge: Sirve para integrar/unificar los cambios realizados en los commits de una rama hacia otra. 

Gestion de Ramas:
***
Mark:
Ahora que ya has creado, fusionado y borrado algunas ramas, vamos a dar un vistazo a algunas herramientas de gestión muy útiles cuando comienzas a utilizar ramas de manera avanzada.

El comando git branch tiene más funciones que las de crear y borrar ramas. Si lo lanzas sin parámetros, obtienes una lista de las ramas presentes en tu proyecto:

$ git branch
  iss53
* master
  testing
***

***
Adriana:
***
Fijate en el carácter * delante de la rama master: nos indica la rama activa en este momento (la rama a la que apunta HEAD). 
Si hacemos una confirmación de cambios (commit), esa será la rama que avance. Para ver la última confirmación de cambios en cada rama, 
puedes usar el comando git branch -v:

$ git branch -v
  iss53   93b412c fix javascript issue
* master  7a98805 Merge branch 'iss53'
  testing 782fd34 add scott to the author list in the readmes
Otra opción útil para averiguar el estado de las ramas, es filtrarlas y mostrar solo aquellas que han sido fusionadas (o que no lo han sido) con la rama actualmente activa. Para ello, Git dispone de las opciones --merged y --no-merged. 
Si deseas ver las ramas que han sido fusionadas con la rama activa, puedes lanzar el comando git branch --merged:

$ git branch --merged
  iss53
* master

***
Daniel
***
Aparece la rama iss53 porque ya ha sido fusionada. Las ramas que no llevan por delante el carácter * pueden ser eliminadas sin problemas, porque todo su contenido ya ha sido incorporado a otras ramas.

Para mostrar todas las ramas que contienen trabajos sin fusionar, puedes utilizar el comando git branch --no-merged:

$ git branch --no-merged
  testing
Esto nos muestra la otra rama del proyecto. Debido a que contiene trabajos sin fusionar, al intentar borrarla con git branch -d, el comando nos dará un error:

$ git branch -d testing
error: The branch 'testing' is not fully merged.
If you are sure you want to delete it, run 'git branch -D testing'.
Si realmente deseas borrar la rama y perder el trabajo contenido en ella, puedes forzar el borrado con la opción -D; tal y como indica el mensaje de ayuda.

