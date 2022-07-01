FROM centos:7.6.1810

LABEL maintainer="zhoulouzi@hotmail.com"

ENV LANG en_US.UTF-8

RUN rm -rf /etc/localtime \
    && ln -s /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN yum -y install \
           which \
           openssl \
           openssl-devel \
           telnet \
           strace \
           zip \
           unzip \
           tcpdump \
           ethtool \
           net-tools \
           iotop \
           iproute \
           yum-utils \
           wget \
           curl \
           sysstat \
           less \
           bind-utils && \
    yum clean all
