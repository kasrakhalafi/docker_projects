# docker_projects
These projects are the implementations of the Udemy course [Docker and Kubernetes: The Complete Guide](https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/?couponCode=KEEPLEARNING).

# Project 1
In the first project, a tiny Node.js web application is created, wrapped inside of a Docker container, and accessed the web application from a browser running on the local machine.

In order to build the image, the following command is used:
```bash
docker build -t kasrraaaaa/simpleweb:latest .
```
In order to run the container in this project, the following command is used:
```bash
docker run -p 8080:8080 kasrraaaaa/simpleweb
```
where the first port number is the port number of the host machine and the second port is the port inside the container.

# Project 2

In the second project, a Docker container contains a web application where the number of visits to the server is displayed inside the browser.
In this project, Docker containers
for both the Node application and the Redis server are separated, where the Redis server keeps track of the number of visits.

In order to connect the containers in an automated manner, the docker-compose is used. We also use docker-compose to restart the crashed and stopped containers.
In order to start the containers, the following command is used:
```bash
docker-compose up --build
```

To stop the docker-compose, the following command is used:
```bash
docker-compose down
```
