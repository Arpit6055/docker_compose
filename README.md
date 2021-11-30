# docker_compose
Creating docker images using docker compose service 

Docker Compose is a tool that was developed to help define and share multi-container applications. With Compose, we can create a YAML file to define the services and with a single command, can spin everything up or tear it all down

## Installation
first install [docker](https://www.docker.com/products/docker-desktop) on your machine.

 Now download the source code. 

open your terminal and open this directory 

## Usage

```CMD
docker-compose up
```
# Or
```CMD
docker-compose up --scale web=10
```

Remember not to mention port in any of the services which you might want to scale up, because then it will assign the same port to all the conatiner service


This will start binding everything up and will spin up both the containers mentioned in .yml file. The db service will spin up fist as the web service mentioned in the .yml file is dependent on db service

