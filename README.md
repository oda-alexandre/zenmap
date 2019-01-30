# ZENMAP

![zenmap](https://raw.githubusercontent.com/oda-alexandre/zenmap/master/img/logo-zenmap.png) ![docker](https://raw.githubusercontent.com/oda-alexandre/zenmap/master/img/logo-docker.png)


## INDEX

- [Build Docker](#BUILD)
- [Introduction](#INTRODUCTION)
- [Prerequis](#PREREQUIS)
- [Installation](#INSTALLATION)
- [License](#LICENSE)


## BUILD DOCKER

[![zenmap docker build](https://img.shields.io/docker/build/alexandreoda/zenmap.svg)](https://hub.docker.com/r/alexandreoda/zenmap)


## INTRODUCTION

Ce repository contient le fichier Dockerfile de [zenmap](https://nmap.org/zenmap) pour [Docker](https://www.docker.com), mis à jour automatiquement dans le [Docker Hub](https://hub.docker.com/r/alexandreoda/zenmap/) public.


## PREREQUIS

Installer [Docker](https://www.docker.com)


## INSTALLATION

```
docker run -d --name zenmap -v ${HOME}:/home/zenmap -v /tmp/.X11-unix/:/tmp/.X11-unix/ -v ${XAUTHORITY}:/xauthority:ro -e XAUTHORITY='/xauthority' -e DISPLAY alexandreoda/zenmap
```


## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://github.com/oda-alexandre/zenmap/blob/master/LICENSE)
