FROM zhoulouzi/java:jdk-8u251

LABEL maintainer="zhoulouzi@hotmail.com"

ENV MAVEN_VERSION 3.6.3

RUN mkdir -p /usr/share/maven /usr/share/maven/ref \
  && curl -fsSL -o /tmp/apache-maven.tar.gz https://apache.osuosl.org/maven/maven-3/${MAVEN_VERSION}/binaries/apache-maven-${MAVEN_VERSION}-bin.tar.gz \
  && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1 \
  && rm -f /tmp/apache-maven.tar.gz \
  && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn \
  && mkdir /root/.m2

# ADD settings.xml /usr/share/maven/conf/settings.xml

ENV MAVEN_HOME /usr/share/maven
