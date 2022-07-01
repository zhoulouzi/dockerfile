FROM zhoulouzi/centos:7.6-base

LABEL maintainer="zhoulouzi@hotmail.com"

ENV DOCKER_VERSION 19.03.7

ADD docker-ce.repo /etc/yum.repos.d/docker-ce.repo

RUN yum install -y containerd.io-$DOCKER_VERSION \
                   docker-ce-$DOCKER_VERSION \
                   docker-ce-cli-$DOCKER_VERSION \
    yum clean all
