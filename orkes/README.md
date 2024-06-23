# Orkes Conductor

Netflix Conductor officially stopped supporting the conductor project and Orkes now maintains it.

It is almost same as the Netflix one.

The differences I found:
- Conductor spring boot app jar was readily available, whereas for Orkes conductor, I couldn't find one. Instead, they've provided a docker image which consists of the Consuctor Spring Boot app as well as the Frontend app
- Orkes Conductor also has a hosted playground
- The workflow json from Netflix conductor almost worked in Orkes conductor as it is (it required an additional field `schemaVersion`)



### Setup

The Orkes conductor Docker image can be run using the command

```
docker run --init -p 8080:8080 -p 1234:5000 --mount source=redis,target=/redis --mount source=postgres,target=/pgdata orkesio/orkes-conductor-community-standalone:latest
```


> FYI, this is the Dockerfile used for building the Orkes conductor image : https://github.com/orkes-io/orkes-conductor-community/blob/main/docker/DockerfileStandalone


Also, if you want to get the conductor server jar from the docker container, you can use the following command:
```
docker cp <container-id>:/app/libs/server.jar .
```
