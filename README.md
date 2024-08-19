
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
## Merge y resolucion de conflitos
### **¿Cómo **resolver conflictos** de fusión en **Git**?**

1.  Abra el archivo en su editor de texto preferido.

2.  Identificar los cambios que causan el **conflicto** y hacer los cambios necesarios.

3.  Use "**git** add conflict. txt" para organizar el archivo.

4.  Usa "**git** commit -m 'su mensaje de confirmación aquí'" comprometerse.
