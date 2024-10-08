
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
###Peticion de Cambio (Pull Request)
 
Que es 

Un Pull Request es una función de GitHub que permite a tu equipo solicitar la revisión y aprobación de sus cambios antes de fusionarlos en la rama principal de desarrollo, denominada “master” o “main”.  

Funcionamiento
1. Usuario 1 realiza cambios en el archivo base en su repositorio local
2. Hace push a su branch
3. Solicita una Peticion de Cambio
4. El equipo verifica el codigo
5. Se hace merge
--------------------------------------------------------------------------------------------------------------------

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
modificaciones necesarias. Luego, sube los cambios al repositorio remoto usando git push origin <rama
                                                                                                      
¿Como corregir un Pull Request?


Al revisar un pull request, es posible encontrar problemas o áreas que necesiten corrección antes de que los cambios se puedan unir con la rama principal. Aquí se explica cómo corregir un pull request de forma efectiva.

1. Lee los comentarios y feedback

2. Regresa a tu rama local: Utiliza el comando git checkout <rama> para volver a la rama en la que realizaste los cambios y necesitas revisar.

3. Realiza las modificaciones

4. Realiza un nuevo commit: Después de efectuar las correcciones, utiliza el comando git commit -am '<Comentario>'

5. Sube los cambios al repositorio remoto: Utiliza el comando git push origin <rama>

6. Actualiza el pull request
                                                                                                      

## Merge y resolucion de conflitos
### **¿Cómo **resolver conflictos** de fusión en **Git**?**

1.  Abra el archivo en su editor de texto preferido.

2.  Identificar los cambios que causan el **conflicto** y hacer los cambios necesarios.

3.  Use "**git** add conflict. txt" para organizar el archivo.

4.  Usa "**git** commit -m 'su mensaje de confirmación aquí'" comprometerse.

El merge se puede hacer de forma automática o manual. Si Git detecta que los cambios en las dos ramas no interfieren entre sí. 

# Forks
![alt text](https://s3.ap-south-1.amazonaws.com/s3.studytonight.com/tutorials/uploads/pictures/1625217336-103268.png "git Forks") 

## Introducción

Los forks o bifurcaciones son una característica única de GitHub en la que se crea una copia exacta del estado actual de un repositorio directamente en GitHub. Este repositorio podrá servir como otro origen y se podrá clonar (como cualquier otro repositorio). En pocas palabras, lo podremos utilizar como un nuevo repositorio git cualquiera
Un fork es como una bifurcación del repositorio completo. Comparte una historia en común con el original, pero de repente se bifurca y pueden aparecer varios cambios, ya que ambos proyectos podrán ser modificados en paralelo y para estar al día un colaborador tendrá que estar actualizando su fork con la información del original.


Al hacer un fork de un poryecto en GitHub, te conviertes en dueñ@ del repositorio fork, puedes trabajar en este con todos los permisos, pero es un repositorio completamente diferente que el original, teniendo solamente alguna historia en común (como crédito al creado o creadora original).
Los forks son importantes porque es la manera en la que funciona el open source, ya que, una persona puede no ser colaborador de un proyecto, pero puede contribuír al mismo, haciendo mejor software que pueda ser utilizado por cualquiera.


```
git remote add <nombre_del_remoto> <url_del_remoto> 
git remote upstream https://github.com/freddier/hyperblog
```

Al crear un remoto adicional, podremos hacer pull desde el nuevo origen. En caso de tener permisos, podremos hacer fetch y push.

```
git pull <remoto> <rama>
git pull upstream master
```
Este pull nos traerá los cambios del remoto, por lo que se estará al día en el proyecto. El flujo de trabajo cambia, en adelante se estará trabajando haciendo pull desde el upstream y push al origin para pasar a hacer pull request.
```
git pull upstream master
git push origin master
```
