# MySQL

MySQL server running on Ubuntu 18.04.

## Build Image

```
docker build -t mysql-ubuntu:latest .
```

## Run Container

```
docker run -p 3306:3306 -e MYSQL_ROOT_PASSWORD=[Root Password Here] --name mysql-ubuntu -d mysql-ubuntu:latest
```

* With volume mapping

```
docker run -p 3306:3306 -e MYSQL_ROOT_PASSWORD=[Root Password Here] -v [Volume Directory Here]:/var/lib/mysql --name mysql-ubuntu -d mysql-ubuntu:m5.7-u18.04
```

## MySQL connection from host

```
mysql -h 127.0.0.1 -P 3306 -u root -p
```
