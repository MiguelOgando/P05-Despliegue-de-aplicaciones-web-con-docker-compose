# MediaWiki
## Pasos para docker-compose
> docker-compose up -d 

paramos el compose y ponemos el siguiente comando:

> docker-compose -f docker-compose.yml up

Accedemos al [localhost](http://localhost:8082)

En caso de tener que volver a realizar la instalación por error del IpAddress, haremos lo siguiente:
*   Eliminamos el LocalSettings actual porque se producirían errores
*   Comentamos la línea 19 [ - ./LocalSettings.php:/var/www/html/LocalSettings.php ]
* > Terminal: docker-compose up -d
*   Hacemos click en empezar la instalación
*   Descargamos el LocalSettings:
    *   Primer paso:
        *   Inspeccionamos mariadb y copiamos el IpAddress que nos indique para hacer la conexión
        *   Base de datos: my_wiki
        *   Usuario: wikimiguel
        *   Contraseña: miguel
    *   Segundo paso:
        *   Nombre: my_wiki
        *   Usuario: Wikimiguel
        *   Contraseña: ejemplo123456789
    *   Tercer paso:
        *   Descargamos el LocalSettings.php
*   Arrastramos/copiamos/cortamos el LocalSettings a la posición del repositorio actual tanto por comando como por acciones del explorador de archivos
*   Paramos el compose y descomentamos la línea 19 [ - ./LocalSettings.php:/var/www/html/LocalSettings.php ]
*   Usamos el comando:
    *   >  docker-compose -f docker-compose.yml up

En caso de errores continuos de la instalación, borrar los volúmenes para que estos se creen nuevamente de forma automática.

### Links de referencia
[Docker hub](https://hub.docker.com/_/mediawiki)
