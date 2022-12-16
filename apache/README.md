# Apache
## Pasos para docker-compose
> docker-compose up -d 

Accedemos al [localhost](http://localhost:8081/)

## Realización paso a paso
Accedemos al [TheServerSide](https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/Simple-Apache-docker-compose-example-with-Dockers-httpd-image) donde encontraremos el código de docker-compose, este deberá ser modificado para que la ruta del volúmen sea válida:

> ./website:/var/www/html

Copiamos el código en nuestro fichero llamado [docker-compose.yml](docker-compose.yml), donde podemos personalizar algunas de las variables del fichero, como el "container_name":

> container_name: miguel-apache-app

En la parte ubicada de "miguel-apache-app".

Accedemoms al terminal y colocamos:
> docker-compose up -d 

Accedemos al [localhost](http://localhost:8081/)

### Link de referencia
[Docker hub](https://hub.docker.com/_/httpd)

[TheServerSide](https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/Simple-Apache-docker-compose-example-with-Dockers-httpd-image)

[StackOverflow](https://stackoverflow.com/questions/41423349/docker-how-to-set-up-apache-php-in-docker-compose-yml)