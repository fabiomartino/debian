# Dockerizing a base images with:
#
#   - Debian Stretch
#   - curl, wget
#
# Build:    docker build -t ermac/debian:stretch-curl .
#
# https://github.com/docker-library/buildpack-deps
#

FROM debian:stretch

MAINTAINER Fabio Martino <fabiomartino@libero.it>

RUN apt-get update && apt-get install -y --no-install-recommends \
        ca-certificates \
        curl \
        wget \
    && rm -rf /var/lib/apt/lists/*