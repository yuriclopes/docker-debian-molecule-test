# Debian with SystemD

[![CI](https://github.com/yuriclopes/docker-debian-systemd/workflows/Build/badge.svg?branch=main&event=push)](https://github.com/yuriclopes/docker-debian-systemd/actions?query=workflow%3ABuild) [![Docker pulls](https://img.shields.io/docker/pulls/yuriclopes/docker-debian-systemd)](https://hub.docker.com/repository/docker/yuriclopes/debian-systemd)

- Debian 11 (Bullseye) Docker container with SystemD.

## Tags

  - `11-slim`: Latest stable version for Bullseye release

## How to Build

This image is built on Docker Hub automatically, but if you need to build the image on your own locally, do the following:

  1. [Install Docker](https://docs.docker.com/engine/installation/).
  2. `cd` into this directory.
  3. Run `docker build -t debian-systemd:11-slim -f 11-slim/Dockerfile .`

## How to Use

  1. [Install Docker](https://docs.docker.com/engine/installation/).
  2. Pull this image from Docker Hub: `docker pull yuriclopes/debian-systemd:11-slim` (or use the image you built earlier, e.g. `debian-systemd:11-slim`).
  3. Run a container from the image: `docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro yuriclopes/debian-systemd:11-slim`.

> **Important Note**: I use this image for molecule testing. Use on production at your own risk!

## Author

Created in 2022 by Yuri Corona Lopes.