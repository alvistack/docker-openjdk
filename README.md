# Docker Image Packaging for OpenJDK

[![GitLab pipeline status](https://img.shields.io/gitlab/pipeline/alvistack/docker-openjdk/master)](https://gitlab.com/alvistack/docker-openjdk/-/pipelines)
[![GitHub release](https://img.shields.io/github/release/alvistack/docker-openjdk.svg)](https://github.com/alvistack/docker-openjdk/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-openjdk.svg)](https://github.com/alvistack/docker-openjdk/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/openjdk-16.svg)](https://hub.docker.com/r/alvistack/openjdk-16)
OpenJDK (Open Java Development Kit) is a free and open source implementation of the Java Platform, Standard Edition (Java SE).
Learn more about OpenJDK: <https://openjdk.java.net/>

## Supported Tags and Respective Packer Template Links

  - [`alvistack/openjdk-16`](https://hub.docker.com/r/alvistack/openjdk-16)
      - [`packer/docker-16/packer.json`](https://github.com/alvistack/docker-openjdk/blob/master/packer/docker-16/packer.json)
  - [`alvistack/openjdk-11`](https://hub.docker.com/r/alvistack/openjdk-11)
      - [`packer/docker-11/packer.json`](https://github.com/alvistack/docker-openjdk/blob/master/packer/docker-11/packer.json)
  - [`alvistack/openjdk-8`](https://hub.docker.com/r/alvistack/openjdk-8)
      - [`packer/docker-8/packer.json`](https://github.com/alvistack/docker-openjdk/blob/master/packer/docker-8/packer.json)

## Overview

This Docker container makes it easy to get an instance of OpenJDK up and running.
Based on [Official Ubuntu Docker Image](https://hub.docker.com/_/ubuntu/) with some minor hack:

  - Packaging by Packer Docker builder and Ansible provisioner in single layer
  - Handle `ENTRYPOINT` with [catatonit](https://github.com/openSUSE/catatonit)

### Quick Start

For the `VOLUME` directory that is used to store the repository data (amongst other things) we recommend mounting a host directory as a [data volume](https://docs.docker.com/engine/tutorials/dockervolumes/#/data-volumes), or via a named volume if using a docker version \>= 1.9.
Start OpenJDK:
\# Pull latest image
docker pull alvistack/openjdk-16
\# Run as detach
docker run   
\-itd   
\--rm   
\--name openjdk   
alvistack/openjdk-16   
java -version

## Versioning

### `YYYYMMDD.Y.Z`

Release tags could be find from [GitHub Release](https://github.com/alvistack/docker-openjdk/releases) of this repository. Thus using these tags will ensure you are running the most up to date stable version of this image.

### `YYYYMMDD.0.0`

Version tags ended with `.0.0` are rolling release rebuild by [GitLab pipeline](https://gitlab.com/alvistack/docker-openjdk/-/pipelines) in weekly basis. Thus using these tags will ensure you are running the latest packages provided by the base image project.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
