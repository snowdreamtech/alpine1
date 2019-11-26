FROM arm32v7/alpine:3.10

LABEL maintainer="snowdream <sn0wdr1am@icloud.com>"

COPY qemu-arm-static /usr/bin

COPY .vimrc /root/

RUN echo @edge http://dl-cdn.alpinelinux.org/alpine/edge/main >> /etc/apk/repositories \
    && echo @edgecommunity http://dl-cdn.alpinelinux.org/alpine/edge/community >> /etc/apk/repositories \
    && echo @testing http://dl-cdn.alpinelinux.org/alpine/edge/testing >> /etc/apk/repositories  \
    && apk add --no-cache vim \ 
    && rm -rf /tmp/* /var/cache/apk/*