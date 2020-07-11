FROM alpine:3.12

ARG VCS_REF
ARG BUILD_DATE

RUN apk update && apk --no-cache add \
  bash \
  curl \
  git \
  ca-certificates \
  gettext \
  bind-tools \
  make \
  jq \
  busybox-extras \
  bind-tools \
  pwgen \
  vim \
  nmap


LABEL org.label-schema.vcs-url="https://github.com/mapitman/dockerfiles/linux-tools"
LABEL maintainer="Mark Pitman <mark@pitman.io>"

CMD [ "/bin/bash" ]
