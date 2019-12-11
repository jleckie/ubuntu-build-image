FROM ubuntu:bionic

ENV DEBIAN_FRONTEND noninteractive

RUN \
  apt-get update && \
  apt-get install -y language-pack-en-base && \
  export LC_ALL=en_US.UTF-8 && \
  export LANG=en_US.UTF-8 && \
  apt-get install -y software-properties-common curl && \
  apt-get install -y python3-pip && \
  apt-get install -y openjdk-8-jre-headless && \
  pip3 install \
    certbot \
    cryptography \
    certbot-dns-cloudflare \
    certbot-dns-cloudxns \
    certbot-dns-digitalocean \
    certbot-dns-dnsimple \
    certbot-dns-dnsmadeeasy \
    certbot-dns-google \
    certbot-dns-luadns \
    certbot-dns-nsone \
    certbot-dns-rfc2136 \
    certbot-dns-route53 && \
  apt-get autoremove -y && \
  rm -rf /var/lib/apt/lists/*
