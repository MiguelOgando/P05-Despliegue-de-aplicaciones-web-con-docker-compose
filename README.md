Todas las pruebas han sido realizadas desde Windows, posiblemente Linux no comparta los mismos comandos en algunos casos.

Cada compose tiene su port personalizado, en caso de fallo revisar que no se está usando el port correspondiente.

# Pasos principales

Iniciar el docker para realizar las acciones indicadas.

Comprobar que no se presentan copias iguales a las del proyecto para no crear interferencias.

Abrir un terminal donde ejecutar todos los comandos necesarios.

Nos situaremos dentro de la carpeta donde queramos ejecutar los comandos (acción recomendada) o en la dirección del archivo por comando.

Para entrar a dichas carpetas será necesario el siguiente comando:
> cd [ruta]

Carpetas creadas para el proyecto:

*   apache - [port](http://localhost:8081/) : 8081
    *   website
    *   docker-compose.yml
    *   README.md 
*   mediawiki - [port](http://localhost:8082/) : 8082
    *   docker-compose.yml
    *   LocalSettings.php
    *   README.md 
*   guestbook - [port](http://localhost:8083/) : 8083
    *   docker-compose.yml
    *   README.md 
*   wordpress - [port](http://localhost:8084/) : 8084
    *   docker-compose.yml
    *   README.md 
*   adminer - [port](http://localhost:8085/) : 8085
    *   docker-compose.yml
    *   README.md 
*   README.md
