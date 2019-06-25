# ZENMAP

<img src="https://s24255.pcdn.co/wp-content/uploads/2013/08/zenmap.png" />

## INDEX

- [Badges](#BADGES)
- [Introduction](#INTRODUCTION)
- [Prerequis](#PREREQUIS)
- [Installation](#INSTALLATION)
- [License](#LICENSE)


## BADGES

[![pipeline status](https://gitlab.com/oda-alexandre/zenmap/badges/master/pipeline.svg)](https://gitlab.com/oda-alexandre/zenmap/commits/master)


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
