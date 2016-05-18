# rpi-alpine-mysql
Raspberry Pi Docker image with minimal GNU/Linux system with Mysql

### Create a Dockerfile

```
FROM hypriot/rpi-alpine-scratch

RUN apk update
RUN apk add mysql-client

ENTRYPOINT ["mysql"]
```

### Build image

`docker build -t alpine-mysql .`
