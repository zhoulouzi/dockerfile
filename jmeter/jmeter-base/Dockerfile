FROM zhoulouzi/java:jdk-8u251

LABEL maintainer="zhoulouzi@hotmail.com"

RUN mkdir /jmeter \
	&& cd /jmeter/ \
	&& wget https://archive.apache.org/dist/jmeter/binaries/apache-jmeter-$JMETER_VERSION.tgz \
	&& tar -xzf apache-jmeter-$JMETER_VERSION.tgz \
	&& rm apache-jmeter-$JMETER_VERSION.tgz

ENV JMETER_HOME /jmeter/apache-jmeter-$JMETER_VERSION/

ENV PATH $JMETER_HOME/bin:$PATH