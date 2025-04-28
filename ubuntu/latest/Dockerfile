FROM ubuntu:24.04

RUN --mount=type=cache,target=/var/cache/apt \
  apt update && \
  apt install git wget unzip
