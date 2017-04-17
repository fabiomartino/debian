# Dockerizing a base images with:
#
#   - Debian Stretch
#   - curl, wget, unzip
#
# Build:    docker build -t ermac/debian:stretch-curl .
#
# https://github.com/docker-library/buildpack-deps
#

FROM debian:stretch

MAINTAINER Fabio Martino <fabiomartino@libero.it>

RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
    apt-utils \
 && rm -rf /var/lib/apt/lists/*

RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
        ca-certificates \
        curl \
        wget \
        unzip \
    && rm -rf /var/lib/apt/lists/*