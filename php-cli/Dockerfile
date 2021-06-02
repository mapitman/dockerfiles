FROM php:7.4-cli-alpine
LABEL   org.label-schema.build-date=$BUILD_DATE \
        org.label-schema.vcs-ref=$VCS_REF \
        org.label-schema.vcs-url="https://github.com/mapitman/dockerfiles/php-cli" \
        maintainer="Mark Pitman https://github.com/mapitman"

RUN apk update && apk add git zip jq make
ADD php.ini /usr/local/etc/php/php.ini
CMD ["/bin/sh"]
