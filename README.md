# ZENMAP

<img src="https://assets.gitlab-static.net/uploads/-/system/project/avatar/12904492/zenmap.png" width="200" height="200"/>


## INDEX

- [ZENMAP](#zenmap)
  - [INDEX](#index)
  - [BADGES](#badges)
  - [FIRST UPDATE](#first-update)
  - [INTRODUCTION](#introduction)
  - [PREREQUISITES](#prerequisites)
  - [INSTALL](#install)
  - [LICENSE](#license)


## BADGES

[![pipeline status](https://gitlab.com/oda-alexandre/zenmap/badges/master/pipeline.svg)](https://gitlab.com/oda-alexandre/zenmap/commits/master)


## FIRST UPDATE

Date: 01-01-01


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

```docker run -d --name zenmap -v ${HOME}:/home/zenmap -v /tmp/.X11-unix/:/tmp/.X11-unix/ -v ${XAUTHORITY}:/xauthority:ro -e XAUTHORITY='/xauthority' -e DISPLAY alexandreoda/zenmap```


## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://gitlab.com/oda-alexandre/zenmap/blob/master/LICENSE)
