Original tutal from those created on YouTube by Jake Wright

# About Docker Compose

Docker compose is a tool for defining and running multi-container Docker applications. All the containers that are run using Docker compose are running on a virtual Docker network, and therefore they can talk to one another using this network.

# Getting started

This directory has the source code. The docker containers configuration is defined in the `docker-compose.yml` file. 

The backend Python API (`product-service`) has its own `Dockerfile` and this project is referenced from the `docker-compose.yml` and is used when starting it up.

To run the application, `cd` into this directory and run 

```
docker-compose up
```

 The product service and the website will start (if necessary, docker-compose will automatically build the containers).

 To shutdown the running containers use `CTRL + C`

 To run the containers in detached mode use

 ```
 docker-compose up -d
 ```

 To view the running containers use 

 ```
 docker ps
 ```

 To stop the running containers (started using detached mode) use

 ```
 docker-compose stop
 ```
