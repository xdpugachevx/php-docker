FROM php:8-cli

RUN apt-get update && apt-get install -y curl git zip \
  && rm -rf /var/lib/apt/lists/*

RUN docker-php-ext-install pdo mysqli pdo_mysql

COPY --from=composer /usr/bin/composer /usr/bin/composer