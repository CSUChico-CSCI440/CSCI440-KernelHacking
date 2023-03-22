FROM ubuntu:22.04
COPY sources.list /etc/apt/sources.list
RUN apt update  && apt -y upgrade
RUN apt install -y build-essential debhelper
# RUN apt install -y build-dep
RUN apt install -y build-dep linux-image-$(uname -r)
RUN apt install -y linux-headers-$(uname -r)
RUN apt source linux-image-$(uname -r)