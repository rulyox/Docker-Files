# MongoDB

## Run Container

```
docker run --name mongodb -v [directory]:/data/db -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=[user] -e MONGO_INITDB_ROOT_PASSWORD=[password] -d mongo
```
