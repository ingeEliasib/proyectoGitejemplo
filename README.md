git config --global user.name "EliasDevs"
git config --global user.email ingenieroeliasibcadena@gmail.com
git config --global  editor

mkdir carpeta_nueva
rm archivo_borrar

rmdir carpeta_para_borrar


area de trabajo	
		añadir add
			area de preparacion
			commit
				repositorio

git init
git status
git add archivo.text
git status
git commit -m "comentario"

--modifcar el archivo
despues de realizar el cambio podemos ver los cambios con 

git diff nombre_documenot.text
--muestra diferencias
--lo pasamos para subir
git add documento.txt
git commint -m "version nueva"

--con git log puedo ver los commit que he realizado sobre el doc

git log
--sobre este log tenemos los commit con un id es imortante este id
porque con ese podemos reversar ejemplo de un id
commit dce72ab4fc694b1a1b9806228e783c3c0e0bf202
 git chekout dce72ab4fc694b1a1b9806228e783c3c0e0bf202


ahroa no existe el git log del commit 2



------ ramas
para crear o ir a una rama se usa git checkout -b rama_nueva_o_irarama
git checkout -b develop

git add . añade varios documentos cuidado con espacios

------------losnuevos documentos estan en la rama pero no el la nueva
si vamos a master podemos verlo
git checkout master

los documentos no estaran  a la vista

si realizamos checkout a develop los veremos de nuevo

git chekout develop


------merge (mergear) combinar la revision final del documento a Master
revisamos en que rama estamos status
git status
git merge develop --esta es la rama de donde traigo archivos
--conflicto
git merge --abort esto retrocede al merge para evitar problemas

para esto usamos este
git rebase develop --sobre escribe y crea los docs
git rebase develop --skip forzar los cambios a los nuevos

----------como saber que rama estamos
git branch


-------para guardar en una zona segura sin afectar principal
git stash  -guarda los cambios de forma segura sin modificar nada pero sin perder cambios
git status
git stash pop --devuelve los cambios realizados en el espacio de programacion ya qye nos epueden ver
git stash save "primer comentario" guardar un comentario
 git stash list muestrara la lista de comentarios realizados

 git stash list
stash@{0}: On master: segunda modificacion diferente total
stash@{1}: On master: primer comentario

si queremos alguna version 
git stash pop stash@{0}

git checkout . no guarda cambios y modifica doto


