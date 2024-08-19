

GIT ALL <NOMBRE DE ARCHIVO>: Escribir el comando git add <archivo> para agregar los cambios de un archivo especifo al staging

git diff hash archivo: compara el archivo actual con el archivo referenciado con el hash
git add: Sirve para agregar todos los cambios realizados en el directorio  donde uno se encuentra al staging.
git add . : ara agregar todos los archivos del directorio actual.
git revert <ID del commit>  esto creara un nuevo commit que deshace los cambios realizados en el commit anterior .




git reset: te permite deshacer cambios sin crear un nuevo commit a diferencia del revert que solo se puede en local 
este se puede ver en servidor
git commit --amend: Se utiliza para modificar el ultimo commit, te permite añadir archivos o cambiar el texto del commit
### Git Diff
Escribir el comando git diff <archivo> y presionar enter. Esto mostrará las diferencias del archivo.
