# MySQL

MySQL 5.7 server running on Ubuntu 18.04.

https://hub.docker.com/repository/docker/rulyox/mysql-ubuntu


## Build Image

```
docker build -t mysql-ubuntu:m5.7-u18.04 .
```

Or download from docker hub

```
docker pull rulyox/mysql-ubuntu
```


## Run Container

```
docker run -p 3306:3306 -e MYSQL_ROOT_PASSWORD=[Root Password Here] --name mysql-ubuntu -d mysql-ubuntu:m5.7-u18.04
```

Or run with volume mapping

```
docker run -p 3306:3306 -e MYSQL_ROOT_PASSWORD=[Root Password Here] -v [Volume Directory Here]:/var/lib/mysql --name mysql-ubuntu -d mysql-ubuntu:m5.7-u18.04
```


## MySQL connection from host

```
mysql -h 127.0.0.1 -P 3306 -u root -p
```
