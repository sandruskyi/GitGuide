# Cargar Proyecto Local en GitHub por consola
Pasos a seguir para subir un proyecto local en GitHub mediante la cmd de Windows

----------------------------------
## Pasos: 
  1) En la cmd ve hasta la carpeta del proyecto que quieras cargar/subir. Puedes utilizar dir para ver tus archivos en la ruta actual y cd para moverte entre rutas. Ejemplo: 
    cd Documentos 
    dir 
    cd MiProyecto
    
  2) git init
  
  3) git add .
     En caso de error puedes usar: 
     git add --ignore-errors .
     
  4) git commit -m "Primer commit del proyecto - Detallalo como quieras."

  5) git remote add origin https://github.com/NOMBRE_USUARIO/NOMBRE_PROYECTO.git

  6) git push -u origin master

