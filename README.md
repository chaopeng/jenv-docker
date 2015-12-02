## jenv-docker

This repository contains **Dockerfile** of [Oracle-Java](https://www.java.com/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/dockerfile/java/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Base Docker Image

* [offical-centos:latest](https://registry.hub.docker.com/_/centos/)
* [offical-alpine:latest](https://hub.docker.com/_/alpine/) for tag: `latest-mini`

### Docker Tags

`chaopeng/jenv` provides multiple tagged images:

* `latest`: oracle-java 1.8.0_60 [![](https://badge.imagelayers.io/chaopeng/jenv:latest.svg)](https://imagelayers.io/?images=chaopeng/jenv:latest 'Get your own badge on imagelayers.io')
* `latest-mini`: alpine + oracle-java 1.8.0_60 [![](https://badge.imagelayers.io/chaopeng/jenv:latest.svg)](https://imagelayers.io/?images=chaopeng/jenv:latest 'Get your own badge on imagelayers.io')
* `jdk8`: oracle-java 1.8.0_60 [![](https://badge.imagelayers.io/chaopeng/jenv:jdk8.svg)](https://imagelayers.io/?images=chaopeng/jenv:jdk8 'Get your own badge on imagelayers.io')
* `jdk7`: oracle-java 1.7.0_75 [![](https://badge.imagelayers.io/chaopeng/jenv:jdk7.svg)](https://imagelayers.io/?images=chaopeng/jenv:jdk7 'Get your own badge on imagelayers.io')

### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/chaopeng/chaopeng/jenv/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull chaopeng/jenv`



### Usage

    docker run -it --rm chaopeng/jenv java -version
    
### To Run a Bash Script

    add `source "/root/.jenv/bin/jenv-init.sh"` to first line.
    
### Thanks

* [jenv.io](http://jenv.io/)

