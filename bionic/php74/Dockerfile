FROM ubuntu:bionic

ENV DEBIAN_FRONTEND noninteractive

RUN \
  apt update && \
  apt install -y language-pack-en-base && \
  export LC_ALL=en_US.UTF-8 && \
  export LANG=en_US.UTF-8 && \
  apt install -y software-properties-common curl && \
  curl -sL https://sentry.io/get-cli/ | bash && \
  add-apt-repository ppa:ondrej/php && \
  apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0xF1656F24C74CD1D8 && \
  apt update && \
  apt install -y \
    php7.4 \
    php7.4-cli \
    php7.4-dev \
    php7.4-bcmath \
    php7.4-common \
    php7.4-curl \
    php7.4-dba \
    php7.4-enchant \ 
    php7.4-gd \
    php7.5-intl
    php7.4-json \
    php7.4-ldap \
    php7.4-mbstring \
    php7.4-mysql \
    php7.4-opcache \
    php7.4-pspell \
    php7.4-readline \
    php7.4-soap \
    php7.4-xml \
    php7.4-zip \
    php7.4-phpdbg \
    php-xdebug \
    php-imagick \
    php-redis \
    composer \
    npm \
    git \
    ruby \
    packaging-dev \
    dh-make \
    git-buildpackage \
    libmariadbclient-dev \
    && \
  apt remove -y software-properties-common && \
  apt autoremove -y && \
  rm -rf /var/lib/apt/lists/*
