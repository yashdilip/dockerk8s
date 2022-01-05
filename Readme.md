## To run the Spring Boot application using Maven
### mvn spring-boot:run

## Build Docker image using Spring Boot built-in support for docker application _(Docker daemon needs to run before)_
### mvn spring-boot:build-image

## List all running docker image the docker container
### docker ps

## List all available docker image/s
### docker image ls

## Run a specific docket image mapped to a port, _use -d param to run the docker in detached mode_
### docker container run -p 8080:8080 dockerk8s

## To stop the running docker image in a container
### docker container stop <container id>

## Remove docker image from docker registry (force)
### docker image rm dockerk8s:0.0.1-SNAPSHOT -f

## Build docker image using Maven
### docker build . --tag k8sdocker

## Using docker-compose.yml file
## (1) Build/Run docker image
### docker-compose up --build
## (2) Stop/remove docker image
### docker-compose down