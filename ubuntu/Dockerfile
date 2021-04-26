FROM ubuntu:latest
RUN sed -i s@/archive.ubuntu.com/@/mirrors.tuna.tsinghua.edu.cn/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update \
        && apt-get upgrade -y \
        && apt-get install vim openssh-server wget curl \
        && /bin/bash