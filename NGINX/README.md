# NGINX

Share configuration file with container.


## Run Container

```
docker run -it -v [Path to default.conf]:/etc/nginx/conf.d/default.conf --net="host" --name nginx-server nginx:stable
```
