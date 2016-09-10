## Supervisor Dockerfile

This repository contains **Dockerfile** of [Supervisor](http://supervisord.org/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/sangargeo/supervisor-docker/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).

### Base Docker Image

* [dockerfile/ubuntu](http://dockerfile.github.io/#/ubuntu)

### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/sangargeo/supervisor/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull sangargeo/supervisor`

   (alternatively, you can build an image from Dockerfile: `docker build -t="sangargeo/supervisor" https://github.com/sangargeo/supervisor`)

### Usage

    docker run -it --rm sangargeo/supervisor

#### Run with custom config directory

    docker run -d -v <config-dir>:/etc/supervisor/conf.d sangargeo/supervisor
