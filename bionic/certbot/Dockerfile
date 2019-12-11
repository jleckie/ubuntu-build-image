FROM ubuntu:bionic

ENV DEBIAN_FRONTEND noninteractive

RUN \
  apt-get update && \
  apt-get install -y language-pack-en-base && \
  export LC_ALL=en_US.UTF-8 && \
  export LANG=en_US.UTF-8 && \
  sudo add-apt-repository ppa:certbot/certbot
  sudo apt-get update
  apt-get install -y software-properties-common curl && \
  apt-get install -y python-certbot python-certbot-dns-route53 openjdk-8-jre-headless && \
  apt-get autoremove -y && \
  rm -rf /var/lib/apt/lists/*
