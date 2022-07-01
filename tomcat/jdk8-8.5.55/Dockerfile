FROM  zhoulouzi/java:jdk-8u251

LABEL maintainer="zhoulouzi@hotmail.com"

ENV TOMCAT_VERSION 8.5.55

RUN mkdir -p /apps/srv/tomcat8  \
  && curl -fsSL -o /tmp/tomcat.tar.gz http://mirror.bit.edu.cn/apache/tomcat/tomcat-8/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz \
  && tar -xzf /tmp/tomcat.tar.gz -C /apps/srv/tomcat8 --strip-components=1 \
  && rm -f /tmp/tomcat.tar.gz

ENV CATALINA_HOME /apps/srv/tomcat8
ENV PATH $CATALINA_HOME/bin:$PATH

EXPOSE 8080

CMD ["catalina.sh", "run"]
