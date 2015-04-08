## jenv-docker

This repository contains **Dockerfile** of [Oracle-Java](https://www.java.com/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/dockerfile/java/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Base Docker Image

* [offical-centos:latest](https://registry.hub.docker.com/_/centos/)

### Docker Tags

`chaopeng/jenv-docker` provides multiple tagged images:

* 'latest': oracle-java 1.8.0_40
* 'jdk8': oracle-java 1.8.0_40
* 'jdk7': oracle-java 1.7.0_75

### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/chaopeng/chaopeng/jenv-docker/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull chaopeng/jenv-docker`



### Usage

    docker run -it --rm chaopeng/jenv-docker java -version
    
### To Run a Bash Script

    add `source "/root/.jenv/bin/jenv-init.sh"` to first line.
