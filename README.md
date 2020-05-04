# Docker Image Packaging for OpenJDK

[![Travis](https://img.shields.io/travis/com/alvistack/docker-openjdk.svg)](https://travis-ci.com/alvistack/docker-openjdk)
[![GitHub release](https://img.shields.io/github/release/alvistack/docker-openjdk.svg)](https://github.com/alvistack/docker-openjdk/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-openjdk.svg)](https://github.com/alvistack/docker-openjdk/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/openjdk.svg)](https://hub.docker.com/r/alvistack/openjdk/)

OpenJDK (Open Java Development Kit) is a free and open source implementation of the Java Platform, Standard Edition (Java SE).

Learn more about OpenJDK: <https://openjdk.java.net/>

## Supported Tags and Respective `Dockerfile` Links

  - [`14`, `latest`](https://github.com/alvistack/docker-openjdk/blob/master/molecule/14/Dockerfile.j2)
  - [`11`](https://github.com/alvistack/docker-openjdk/blob/master/molecule/11/Dockerfile.j2)
  - [`8`](https://github.com/alvistack/docker-openjdk/blob/master/molecule/8/Dockerfile.j2)

## Overview

This Docker container makes it easy to get an instance of OpenJDK up and running.

Based on [Official Ubuntu Docker Image](https://hub.docker.com/_/ubuntu/) with some minor hack:

  - Minimized `Dockerfile` for meta data definition
  - Provision by Ansible and Molecule Docker driver in single layer
  - Handle `ENTRYPOINT` with [tini](https://github.com/krallin/tini)

### Quick Start

For the `VOLUME` directory that is used to store the repository data (amongst other things) we recommend mounting a host directory as a [data volume](https://docs.docker.com/engine/tutorials/dockervolumes/#/data-volumes), or via a named volume if using a docker version \>= 1.9.

Start OpenJDK:

    # Pull latest image
    docker pull alvistack/openjdk
    
    # Run as detach
    docker run \
        -itd \
        --rm \
        --name openjdk \
        alvistack/openjdk \
        java -version

## Versioning

### `alvistack/openjdk:latest`

The `latest` tag matches the most recent [GitHub Release](https://github.com/alvistack/docker-openjdk/releases) of this repository. Thus using `alvistack/openjdk:latest` or `alvistack/openjdk` will ensure you are running the most up to date stable version of this image.

### `alvistack/openjdk:<version>`

The version tags are rolling release rebuild by [Travis](https://travis-ci.com/alvistack/docker-openjdk) in weekly basis. Thus using these tags will ensure you are running the latest packages provided by the base image project.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
