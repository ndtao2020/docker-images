FROM eclipse-temurin:17-jdk-alpine

ENV GRADLE_VERSION 7.5

# get gradle and supporting libs
RUN apk -U add --no-cache bash git curl
RUN curl https://downloads.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip > gradle.zip; \
    unzip gradle.zip; \
    rm gradle.zip; \
    apk update && apk add --no-cache libstdc++ && rm -rf /var/cache/apk/*

ENV PATH=${PATH}:/gradle-${GRADLE_VERSION}/bin

ENTRYPOINT ["/bin/bash"]
