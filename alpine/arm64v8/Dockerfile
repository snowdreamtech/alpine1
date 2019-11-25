FROM arm64v8/alpine:3.10

LABEL maintainer="snowdream <sn0wdr1am@icloud.com>"

COPY qemu-aarch64-static /usr/bin

COPY .vimrc /root/

RUN apk add --no-cache vim