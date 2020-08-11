/* Esta guía irá aumentando. 
   Son comandos que utilizo en mi día a día, y así no se me olvidan. 
   Documentación Oficial: https://git-scm.com/book/es/v2 || https://docs.github.com/es/github/writing-on-github/basic-writing-and-formatting-syntax */

# Guía Rápida de GitHub 
---------------------------------
## Cargar Proyecto Local en GitHub por consola
Pasos a seguir para subir un proyecto local en GitHub mediante la cmd de Windows

### Pasos: 
  1) En la cmd ve hasta la carpeta del proyecto que quieras cargar/subir. Puedes utilizar dir para ver tus archivos o carpetas en la ruta actual y cd para moverte entre rutas. Ejemplo: 
    cd Documentos 
    dir 
    cd MiProyecto
    
  2) git init
  
  3) git add .
     En caso de error puedes usar: 
     git add --ignore-errors .
     
  4) git commit -m "Title - Primer commit del proyecto " -m "Description - Detallalo como quieras."

  5) git remote add origin https://github.com/NOMBRE_USUARIO/NOMBRE_PROYECTO.git

  6) git push -u origin master
  
---------------------------------
## Creación de Tags
Tags: etiquetar (tag) puntos específicos en la historia como importantes.

### Pasos: 
Para crear un nuevo tag sobre el commit actual debes usar el siguiente comando:
  1) git tag v1.0.0
  
Y para publicarlo debes usar el siguiente comando:
  1) git push origin master --tags
  
---------------------------------
## Ramas
Podemos utilizar las ramas, para controlar cambios o para trabajar en diferentes versiones.

### Pasos: 
Crea y te cambia a la rama creada:
  1) git checkout -b BRANCH_NAME
Si requieres regresar a la rama master o cambiarte a otra:
  1) git checkout master
Para fusionar dos ramas, por ejemplo, en la rama master, primero te posicionas en la rama master y mergeas la rama que quieres: 
  1) git checkout master
  2) git merge BRANCH_NAME
  3) Ya fusionada puedes eliminar la rama si así lo requieres:
      git branch -d BRANCH_NAME
Si quieres crear una nueva rama pero no cambiar a ella utiliza: 
  1) git branch "BRANCH_NAME"
Ahora para cambiar: 
  1) git checkout "BRANCH_NAME"
Listar todas las ramas: 
  1) git branch          
Para unir los cambios de la rama master en la otra rama 
  1) git merge master       

Finalmente: 
  git push origin BRANCH_NAME

---------------------------------
## Releases
Versiones. Se basan en tags. 

### Pasos: 
En GitHub: 
 1) Pág. principal del repo
 2) A la derecha: click en Releases o Latest Release
 3) Click en "Draft a new release"
 4) Crear una nueva versión (se basan en tags). Seleeciona la rama que contiene el proyecto. Elija un titulo, descripción, puedes subir archivos binarios. Si no es estable debes marcar "This is a pre-release"
 5) Click en Publish Release
 
---------------------------------
## Clonar un repo por cmd
https://docs.github.com/es/github/creating-cloning-and-archiving-repositories/cloning-a-repository
