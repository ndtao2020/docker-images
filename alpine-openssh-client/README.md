
# Building image
Clone this repository and then run:
```
docker build -t alpine-openssh-client:latest .
```
# Push to Hub
You can push a new image to this repository using the CLI:
```
docker tag alpine-openssh-client:latest taoqn/alpine-openssh-client:latest
docker push taoqn/alpine-openssh-client:latest
```
