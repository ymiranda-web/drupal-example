ARG BASE_IMAGE
FROM ghcr.io/codebytes-dev/drupal-k8s:9.3.x-base

LABEL maintainer="Luis Yair Miranda Gonzalez <contacto@yairmiranda.com>"

WORKDIR /var/www

COPY ./composer.* .

RUN composer install  --optimize-autoloader --no-interaction --no-progress

COPY . .
