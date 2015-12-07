# docker-ubuntu
A base Ubuntu Docker container with en_AU (UTF8) locale support and timezone set to Australia/Sydney.

The [_deboostrap_ Docker Ubuntu variant](https://hub.docker.com/_/ubuntu-debootstrap/) is used to build these images.

This image is automatically built via the Docker Hub and is available at [chinthakagodawita/ubuntu](https://hub.docker.com/r/chinthakagodawita/ubuntu/).

Its intended use is for Docker container projects that are built on CI tools (such as CircleCI) that run on LXC. These can't reconfigure locale information due to their security setups.

## Available Images

* Ubuntu 14.04
    - `chinthakagodawita/ubuntu:14.04`
    - `chinthakagodawita/ubuntu:latest`
* Ubuntu 12.04
    - `chinthakagodawita/ubuntu:12.04`

## Building
```bash
docker build -t chinthakagodawita/ubuntu:14.04 14.04/
docker build -t chinthakagodawita/ubuntu:12.04 12.04/
```
