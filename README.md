
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




-----------------------------------------------------------------------------------------------------------------------


¿Como corregir un Pull Request?

Al revisar un pull request, es posible encontrar problemas o áreas que necesiten corrección antes de que los cambios se puedan unir con la rama principal. Aquí se explica cómo corregir un pull request de forma efectiva.

1. Lee los comentarios y feedback

2. Regresa a tu rama local: Utiliza el comando git checkout <rama> para volver a la rama en la que realizaste los cambios y necesitas revisar.

3. Realiza las modificaciones

4. Realiza un nuevo commit: Después de efectuar las correcciones, utiliza el comando git commit -am '<Comentario>'

5. Sube los cambios al repositorio remoto: Utiliza el comando git push origin <rama>

6. Actualiza el pull request
