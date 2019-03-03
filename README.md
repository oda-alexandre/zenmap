# ZENMAP

[![dockeri.co](https://dockeri.co/image/alexandreoda/zenmap)](https://hub.docker.com/r/alexandreoda/zenmap)


## INDEX

- [Badges](#BADGES)
- [Introduction](#INTRODUCTION)
- [Prerequis](#PREREQUIS)
- [Installation](#INSTALLATION)
- [License](#LICENSE)


## BADGES

[![version](https://images.microbadger.com/badges/version/alexandreoda/zenmap.svg)](https://microbadger.com/images/alexandreoda/zenmap)
[![size](https://images.microbadger.com/badges/image/alexandreoda/zenmap.svg)](https://microbadger.com/images/alexandreoda/zenmap")
[![build](https://img.shields.io/docker/build/alexandreoda/zenmap.svg)](https://hub.docker.com/r/alexandreoda/zenmap)
[![automated](https://img.shields.io/docker/automated/alexandreoda/zenmap.svg)](https://hub.docker.com/r/alexandreoda/zenmap)


## INTRODUCTION

Ce repository contient le fichier Dockerfile de

- [zenmap](https://nmap.org/zenmap)

Mis à jour automatiquement dans le [docker hub public](https://hub.docker.com/r/alexandreoda/zenmap/)


## PREREQUIS

Installer [docker](https://www.docker.com)


## INSTALLATION

```
docker run -d --name zenmap -v ${HOME}:/home/zenmap -v /tmp/.X11-unix/:/tmp/.X11-unix/ -v ${XAUTHORITY}:/xauthority:ro -e XAUTHORITY='/xauthority' -e DISPLAY alexandreoda/zenmap
```


## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://github.com/oda-alexandre/zenmap/blob/master/LICENSE)
