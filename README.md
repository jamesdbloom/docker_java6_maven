## Java 1.6 & Maven Dockerfile

This repository contains a **Dockerfile** to create a docker container with Java 1.6, Maven 3.1.1 and git

This **Dockerfile** has been published as a [trusted build](https://hub.docker.com/u/jamesdbloom/docker-java6-maven/) to the public [Docker Registry](https://hub.docker.com/).


### Dependencies

* [dockerfile/ubuntu](http://dockerfile.github.io/#/ubuntu)


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [trusted build](https://hub.docker.io/u/jamesdbloom/docker-java6-maven/) from public [Docker Registry](https://index.docker.com/): `docker pull jamesdbloom/docker-java6-maven`

   (alternatively, you can build an image from Dockerfile: `docker build -t="jamesdbloom/docker-java6-maven" github.com/jamesdbloom/docker_java6_maven`)


### Usage (two options)

#### 1. Run container and clone git repo into container

    docker run -i -t -name docker-java6-maven -rm jamesdbloom/docker-java6-maven

    git clone <your repo url>

#### 2. Run container with git repo attached container (from host OS)

    docker run -i -t -name docker_java6_maven -rm -v <your git repo directory>:/volume/git jamesdbloom/docker_java6_maven
    
[James D Bloom](http://blog.jamesdbloom.com)
