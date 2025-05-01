FROM ubuntu:24.04

ENV NODE_VERSION=22.15.0

RUN --mount=type=cache,target=/var/cache/apt \
  apt update && \
  apt install -y git wget unzip curl xz-utils jq && \
  apt clean && \
  rm -rf /var/lib/apt/lists/*

# node
RUN wget https://nodejs.org/dist/v${NODE_VERSION}/node-v${NODE_VERSION}-linux-x64.tar.xz && \
  tar -xvf node-v${NODE_VERSION}-linux-x64.tar.xz && \
  cp node-v${NODE_VERSION}-linux-x64/bin/* /usr/local/bin
