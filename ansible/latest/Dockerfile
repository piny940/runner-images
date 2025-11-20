FROM ghcr.io/piny940/ubuntu-latest:v25

RUN --mount=type=cache,target=/var/cache/apt \
  apt update && \
  apt install -y software-properties-common && \
  add-apt-repository --yes --update ppa:ansible/ansible && \
  apt install -y ansible python3-passlib && \
  apt clean && \
  rm -rf /var/lib/apt/lists/*
