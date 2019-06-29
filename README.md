# ZENMAP

<img src="https://s24255.pcdn.co/wp-content/uploads/2013/08/zenmap.png" />

## INDEX

- [Badges](#BADGES)
- [Introduction](#INTRODUCTION)
- [Prerequisites](#PREREQUISITESITES)
- [Install](#INSTALL)
- [License](#LICENSE)


## BADGES

[![pipeline status](https://gitlab.com/oda-alexandre/zenmap/badges/master/pipeline.svg)](https://gitlab.com/oda-alexandre/zenmap/commits/master)


## INTRODUCTION

Docker image of :

- [zenmap](https://nmap.org/zenmap)

Continuous integration on :

- [gitlab](https://gitlab.com/oda-alexandre/zenmap/pipelines)

Automatically updated on :

- [docker hub public](https://hub.docker.com/r/alexandreoda/zenmap/)


## PREREQUISITES

Use [docker](https://www.docker.com)


## INSTALL

```
docker run -d --name zenmap -v ${HOME}:/home/zenmap -v /tmp/.X11-unix/:/tmp/.X11-unix/ -v ${XAUTHORITY}:/xauthority:ro -e XAUTHORITY='/xauthority' -e DISPLAY alexandreoda/zenmap
```


## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://gitlab.com/oda-alexandre/zenmap/blob/master/LICENSE)
