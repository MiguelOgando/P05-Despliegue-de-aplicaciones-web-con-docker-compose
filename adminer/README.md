# Adminer
## Pasos para docker-compose
> docker-compose up -d 

otra forma de ejecutarlo

> docker-compose -f docker-compose.yml up

Accedemos al [localhost](http://localhost:8085/)

Una vez dentro de la web escribimos los datos:
- Usuario: root
- Contraseña: miguel

## Realización paso a paso
Accedemos al [link](https://hub.docker.com/_/adminer) de referencia para ubicarnos en la sección de la página "How to use this image" donde encontraremos el código de docker-compose.

Copiamos el código en nuestro fichero llamado [docker-compose.yml](docker-compose.yml), donde podemos personalizar algunas de las variables del fichero.

Dentro del fichero, en la base de datos "db", la sección de "environment" puede ser modificada...
> MYSQL_ROOT_PASSWORD: example

En la ubicación de "example".

Abrimos el terminal en la ubicación del archivo y escribimos o copiamos el siguiente código:

> docker-compose up -d 

otra forma de ejecutarlo

> docker-compose -f docker-compose.yml up

Con esto nos crea el compose y tenemos acceso a la web creada, a esta accederemos mediente el [localhost](http://localhost:8085/).

Sólo rellenaremos las casillas de un ususario y contraseña, puesto que las demás no son necesarias o ya están completadas, quedando tal que así:
- Sistem: MySQL
- Server: db
- Usuario: root
- Contraseña: miguel
- Database:

### Link de referencia
[Docker hub](https://hub.docker.com/_/adminer)