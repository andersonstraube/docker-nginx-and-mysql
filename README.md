# nginx and Mysql Docker

A simple study project for MBA class using 2 containers: nginx and mysql

### MySQL

* Version 5.7 linux/x86_64
* Root password is `aul@3root`. To change it, change the `MYSQL_ROOT_PASSWORD` in the `docker-compose.yml` file.
* Default database name is `aula03`. To change it, change the `MYSQL_DATABASE` in the `docker-compose.yml` file.
* Create a directory called `volume` inside `./mysql` to maintain database persistence

### NGINX

* Version latest linux/arm64

### Run

You will need to have [Docker Compose][docker-compose] installed. Once it is installed, just run:

```
docker-compose up
```

Or macOS compatibility with arm64:

```
docker-compose --compatibility up --build
```

If this is your first time running this, docker will download the nginx and MySQL images. 
Then both nginx server and MySQL server will startup in separate containers.

### Test index nginx

http://localhost:8080/

[docker-compose]: https://docs.docker.com/compose/