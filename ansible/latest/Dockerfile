FROM ghcr.io/piny940/ubuntu-latest:v18

RUN --mount=type=cache,target=/var/cache/apt \
  apt update && \
  apt install software-properties-common && \
  add-apt-repository --yes --update ppa:ansible/ansible && \
  apt install ansible && \
  apt clean && \
  rm -rf /var/lib/apt/lists/*
