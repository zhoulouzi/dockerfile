FROM zhoulouzi/centos:7.6-base

LABEL maintainer="zhoulouzi@hotmail.com"

ENV NGINX_VERSION nginx-1.16.1-1.el7.ngx

ADD nginx.repo /etc/yum.repos.d/nginx.repo

RUN  yum install -y $NGINX_VERSION && \
    yum clean all

EXPOSE 80

STOPSIGNAL SIGTERM

CMD ["nginx", "-g", "daemon off;"]
