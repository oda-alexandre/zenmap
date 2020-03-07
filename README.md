# ZENMAP

![logo](https://assets.gitlab-static.net/uploads/-/system/project/avatar/12904492/zenmap.png)

## INDEX

- [ZENMAP](#zenmap)
  - [INDEX](#index)
  - [BADGES](#badges)
  - [INTRODUCTION](#introduction)
  - [PREREQUISITES](#prerequisites)
  - [INSTALL](#install)
    - [DOCKER RUN](#docker-run)
    - [DOCKER COMPOSE](#docker-compose)
  - [LICENSE](#license)

## BADGES

[![pipeline status](https://gitlab.com/oda-alexandre/zenmap/badges/master/pipeline.svg)](https://gitlab.com/oda-alexandre/zenmap/commits/master)

## INTRODUCTION

Docker image of :

- [zenmap](https://nmap.org/zenmap)

Continuous integration on :

- [gitlab pipelines](https://gitlab.com/oda-alexandre/zenmap/pipelines)

Automatically updated on :

- [docker hub public](https://hub.docker.com/r/alexandreoda/zenmap/)

## PREREQUISITES

Use [docker](https://www.docker.com)

## INSTALL

### DOCKER RUN

```\
docker run -d \
--name zenmap \
-e DISPLAY \
-e XAUTHORITY='/xauthority' \
-v ${HOME}:/home/zenmap \
-v /tmp/.X11-unix/:/tmp/.X11-unix/ \
-v ${XAUTHORITY}:/xauthority:ro \
alexandreoda/zenmap
```

### DOCKER COMPOSE

```yml
version: "3.7"

services:
  zenmap:
    container_name: zenmap
    image: alexandreoda/zenmap
    restart: "no"
    privileged: false
    environment:
      - DISPLAY
      - XAUTHORITY='/xauthority'
    volumes:
      - "${HOME}:/home/zenmap"
      - "/tmp/.X11-unix/:/tmp/.X11-unix/"
      - "${XAUTHORITY}:/xauthority:ro"
      - "/tmp/.X11-unix/:/tmp/.X11-unix/"
```

## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://gitlab.com/oda-alexandre/zenmap/blob/master/LICENSE)
