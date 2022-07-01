FROM zhoulouzi/centos:7.6-base

LABEL maintainer="zhoulouzi@hotmail.com"

ENV JAVA_VERSION java-1.8.0-openjdk
ENV CENTOS_PACKAGE 1.8.0.222.b03-1.el7

RUN  yum install -y $JAVA_VERSION-$CENTOS_PACKAGE \
                    $JAVA_VERSION-devel-$CENTOS_PACKAGE && \
    yum clean all

ENV JAVA_HOME /usr/lib/jvm/java
ENV PATH $PATH:$JAVA_HOME/bin
