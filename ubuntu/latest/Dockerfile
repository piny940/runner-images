FROM ubuntu:24.04

RUN --mount=type=cache,target=/var/cache/apt \
  apt update && \
  apt install -y git wget unzip
