### MySQL image for Docker

This Dockerifle modifies [docker-library/mysql:5.6@1f430aeee538aec3b51554ca9fc66955231b3563](https://github.com/docker-library/mysql/tree/1f430aeee538aec3b51554ca9fc66955231b3563/5.6) a little.
#### Quick Start

Run the mysql image

```
$ docker run --name mysql -p 3306:3306 -d -v /opt/mysql/data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=password making/mysql
```

You can access the mysql server as the root user using the following command:

```
$ docker run -it --rm --volumes-from=mysql making/mysql mysql -uroot -p
```
