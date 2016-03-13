FROM ubuntu:trusty

ENV DEBIAN_FRONTEND noninteractive

RUN \
  apt-get update && \
  apt-get install -y python-software-properties software-properties-common && \
  add-apt-repository ppa:ondrej/php5 && \
  apt-get update && \
  apt-get install -y \
    php5 \
    php5-cli \
    php5-common \
    php5-curl \
    php5-dev \
    php5-gd \
    php5-ldap \
    php5-mysql \
    php5-pspell \
    php5-sybase \
    php5-imagick \
    php5-imap \
    php-pear \
    php5-redis \
    php5-json && \
  rm -rf /var/lib/apt/lists/*
