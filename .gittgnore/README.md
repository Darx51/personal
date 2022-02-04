git --version
- muestra la version

pwd
- me muestra donde estoy ubicado

ls -l
- muestra directorios con sus propiedades

git init
- crea un repositorio

git status
- muestra que archivos tengo agregados o sin agregar al staging area

git commit
- creamos un commit o nota:
  i: para insertar texto
  esc:wq  => para salir del commit

git config --global user.email "usuario@etc..mail.com" 
- OJO con las "" incluidas es para configurar correo global la primera vez, si git no sabe quien va a editar el repositorio

git config --global user.name "Nombre de Usuario"
- OJO con las "" incluidas es para configurar usuario

git log
- nos muestra los commits creados 

git checkout -- archivo_a_revertir_Cambios
- revierte cambios de un archivo

git checkout -- .
-todos mis archivos van a ser reconstruidos a como estaban en el ultimo commit 

.gitignore
- asi debo llamar a la carpeta que contendra los archivos que seran ignorados

git commit -m "creacion de commit sin tener que entrar a la consola"

git commit --amend
- edita el ultimo commit

git branch "muestra la rama actual"

git checkout -b rama2
- crea la nueva rama2 

git checkout rama2
- entramos a la rama2 OJO (los archivos creados en la rama2 seran visibles en la rama master hasta que se agreguen al stage, despues de esto ya no se veran en master pero cada cambio que se haga en la rama2 se debera agregar al stage y commitear  poder cambiar a la rama master otra vez)

git branch
- muestra todas las ramas existentes

git add .
- me agrega todos los archivos al stage (debemos tener los archivos ignorados ya dentro de la carpeta .gitignore si no tambien los agregara independiente que sean de otra rama)

git reset .
- revierte o quita todos los archivos del stage

git reset HEAD archivo_A_Sacar_del_Stage.html
- saca del stage el archivo indicado

git checkout HEAD <nomrbeDeArchivo>
- si borraste un archivo sin confirmarlo, este comando lo recupera

git reset --hard HEAD~1
- Si has eliminado un archivo y lo has confirmado

git revert --no-commit <commit>
-si eliinaste un archivo lo confirmaste y lo enviaste a un servidor remoto

git branch -d <rama a eliminar>
-elimina la rama indicada pero se debe hacer merge con la rama master antes

git branch -D <rama a eliminar>
-elimina la rama sin importar si se hizo merge con la rama master

rm -rf .git
- elimina un repositorio, este comando eliminara la carpeta .git

git commit -am "subido al Stage y commit agregado al mismo tiempo"  
- sube al stage y crea el comit al mismo tiempo
  
git push <nombre del repositorio remoto en github>














A = added
M = modified
U = unstaged
D = deleted



