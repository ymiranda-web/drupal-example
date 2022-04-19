FROM ghcr.io/ymiranda-web/docker-templates:7.4-c2-base

LABEL maintainer="Luis Yair Miranda Gonzalez <contacto@yairmiranda.com>"

USER noroot

COPY ./composer.* .

RUN composer install  --optimize-autoloader --no-interaction --no-progress

COPY --chown=noroot . .
