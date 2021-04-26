FROM ubuntu:latest
RUN sed -i s@/archive.ubuntu.com/@/mirrors.163.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update \
        && apt-get upgrade -y \
        && apt-get install vim openssh-server wget curl \
        && /bin/bash