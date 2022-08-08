# Introduction
Docker image used to build projects

# Building image
Clone this repository and then run:
```
docker build -t temurin-17-jdk-maven:latest -t temurin-17-jdk-maven:3.8.6-alpine .
```

# Push to Hub
You can push a new image to this repository using the CLI:
```
docker tag temurin-17-jdk-maven:latest taoqn/temurin-17-jdk-maven:latest
docker push taoqn/temurin-17-jdk-maven:latest

docker tag temurin-17-jdk-maven:3.8.6-alpine taoqn/temurin-17-jdk-maven:3.8.6-alpine
docker push taoqn/temurin-17-jdk-maven:3.8.6-alpine
```
