# Webserver with Apache and PHP on Ubuntu
Docker image with PHP

# How to use
###### Using docker in command line
```
docker run -d -v [host_path]:/var/www/html -p [host_port]:80 edersondev/php:7.3
```

###### Using docker-compose
```
version: '3'
services:
  webphp:
    image: edersondev/php:7.3
    ports:
      - "[host_port]:80"
    volumes:
      - [host_path]:/var/www/html

```