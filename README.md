# Introduction docker-images
Docker image used to build projects with [gradle](https://gradle.org). Similar to [maven](https://hub.docker.com/_/maven/).

# Building image
Clone this repository and then run:
```
docker build -t temurin-17-jdk-gradle:latest -t temurin-17-jdk-gradle:7.5-alpine .
```

# Push to Hub
You can push a new image to this repository using the CLI:
```
docker tag temurin-17-jdk-gradle:latest taoqn/temurin-17-jdk-gradle:latest
docker push taoqn/temurin-17-jdk-gradle:latest

docker tag temurin-17-jdk-gradle:7.5-alpine taoqn/temurin-17-jdk-gradle:7.5-alpine
docker push taoqn/temurin-17-jdk-gradle:7.5-alpine
```
