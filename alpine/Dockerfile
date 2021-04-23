FROM alpine:latest
RUN echo "https://mirror.tuna.tsinghua.edu.cn/alpine/latest-stable/main/" > /etc/apk/repositories

RUN apk update \
        && apk upgrade \
        && apk add --no-cache bash \
        bash-doc \
        bash-completion \
        openrc \
        vim \
        && rm -rf /var/cache/apk/* \
        && /bin/bash