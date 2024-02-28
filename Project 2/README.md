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
