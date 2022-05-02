# docker-gs-ping


Build working example
```
# set Dockerfile to
# FROM golang:1.17-buster AS build
# set go.mod to
# go 1.17
# run below commands
docker build -t docker-gs-ping:1.17 .
trivy image --list-all-pkgs --format json docker-gs-ping:1.17
```

Build not working example
```
# set Dockerfile to
# FROM golang:1.18-buster AS build
# set go.mod to
# go 1.18
# run below commands
docker build -t docker-gs-ping:1.18 .
trivy image --list-all-pkgs --format json docker-gs-ping:1.18
```