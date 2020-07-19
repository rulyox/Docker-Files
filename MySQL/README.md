# MySQL

## Run Container

```
docker run -p 3306:3306 -e MYSQL_ROOT_PASSWORD=[Root Password] -v [Volume Directory]:/var/lib/mysql --name mysql -d mysql
```

## MySQL connection from host

```
mysql -h 127.0.0.1 -P 3306 -u root -p
```
