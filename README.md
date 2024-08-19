
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











--------------------------------------------------------------------------------------------------------------------

parte Daniel:

Cómo hacer un pull request
Un PR es un proceso crucial para facilitar la revisión y la integración efectiva del código.
1. Crea una rama paralela: Antes de hacer cambios en el código, utiliza el comando git checkout -b <rama> 
para crear una nueva rama. Así, podrás hacer tus modificaciones sin afectar la rama principal (por ejemplo, master).

2. Realiza commits: Después de hacer cambios en los archivos, usa git commit -am '<Comentario>' 
para hacer un commit con un mensaje descriptivo.

3. Sube los cambios: Usa git push origin <rama> para subir tus cambios de la rama local al repositorio remoto. 
Reemplaza <rama> con el nombre de tu rama.

4. Crea un pull request: En el repositorio remoto (como GitHub), crea un nuevo pull request. 
Selecciona la rama principal como destino y tu rama con los cambios como comparación.

5. Feedback: Los revisores examinarán los cambios. Usa la sección de comentarios del pull request 
para discutir los cambios y proporcionar feedback adicional.

6. Realiza los cambios solicitados: Si se solicitan cambios, regresa a tu rama local y haz las 
modificaciones necesarias. Luego, sube los cambios al repositorio remoto usando git push origin <rama>.
