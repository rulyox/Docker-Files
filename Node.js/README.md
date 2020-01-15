# Node.js


## Copy files to container

Use Dockerfile inside `copy`.

Node.js files should be in the same directory as Dockerfile. (Use `.dockerignore`.)

### Build Image

```
docker build -t nodejs-copy .
```

### Run Container

```
docker run -it --name nodejs nodejs-copy
```


## Share files with container

Use Dockerfile inside `volume`.

### Build Image

```
docker build -t nodejs-volume .
```

### Run Container

```
docker run -it -v [Host Directory]:/app -w /app --name nodejs nodejs-volume
```
