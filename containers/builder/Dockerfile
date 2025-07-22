FROM docker.io/amd64/ubuntu:24.04

USER root

ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Etc/UTC

RUN apt-get update -yqq \
    && apt-get install -yqq curl \
    && sh -c "$(curl -fsSL https://taskfile.dev/install.sh)" -- -d

WORKDIR /root
