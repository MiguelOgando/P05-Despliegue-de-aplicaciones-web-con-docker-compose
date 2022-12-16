# WordPress
## Pasos para docker-compose
> docker-compose up -d 

otra forma de ejecutarlo

> docker-compose -f docker-compose.yml up

Accedemos al [localhost](http://localhost:8084)

Colocamos los datos correspondientes para loguearnos en la web, estos datos se encuentran tanto en el docker-compose.yml como en wordpress al inspeccionarlo.

*   Título: MiguelOgando
*   Usuario: migueluser
*   Contraseña: miguelpass

Al colocar la contraseña pondrá que es básica por lo que tendremos que pulsar que acepte la contraseña igualmente y seguimos con el inicio de sesión.

## Realización paso a paso
Accedemos al [link](https://hub.docker.com/_/wordpress) de referencia para copiar el código de docker-compose en donde personalizaremos algunas variables si lo deseamos:
>       environment: (wordpress)
    WORDPRESS_DB_USER: migueluser
    WORDPRESS_DB_PASSWORD: miguelpass
    WORDPRESS_DB_NAME: migueldb

>       environment: (db)    
    MYSQL_DATABASE: migueldb
    MYSQL_USER: migueluser
    MYSQL_PASSWORD: miguelpass

Podrán ser modificadas pero con el requerimiento de que sean iguales tanto "wordpress" como "db", [ variable : parte modificable ]

Accedemos al terminal:
> docker-compose up -d 

otra forma de ejecutarlo

> docker-compose -f docker-compose.yml up

Accedemos al [localhost](http://localhost:8084)

Una vez dentro de la web nos pediran 2 registros. El primero para registrarnos y el segundo para iniciar sesión.

En la primera parte colocamos los siguientes datos:

*   Título: MiguelOgando
*   Usuario: migueluser
*   Contraseña: miguelpass
    *   Aceptamos que nos permita crear la cuenta si la contraseña es básica
*   Email: ejemplo@educa.madrid.org

Iniciamos sesión con los datos anteriores que nos pidan.

### Links de referencia
[Docker hub](https://hub.docker.com/_/wordpress)