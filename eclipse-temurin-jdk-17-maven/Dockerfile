FROM eclipse-temurin:17-jdk-alpine

ENV MAVEN_VERSION 3.8.6

RUN apk -U add --no-cache bash git curl tar
RUN mkdir -p /usr/share
RUN curl -fsSL https://repo.maven.apache.org/maven2/org/apache/maven/apache-maven/$MAVEN_VERSION/apache-maven-$MAVEN_VERSION-bin.tar.gz | tar xzf - -C /usr/share
RUN mv /usr/share/apache-maven-$MAVEN_VERSION /usr/lib/mvn
RUN ln -s /usr/lib/mvn/bin/mvn /usr/bin/mvn

RUN apk update && apk add --no-cache libstdc++ && rm -rf /var/cache/apk/*

ENV MAVEN_HOME /usr/lib/mvn
ENV PATH $MAVEN_HOME/bin:$PATH

ENTRYPOINT ["/bin/bash"]
