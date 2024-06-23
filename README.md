# Conductor


### Introduction

Conductor is a free and open-source microservice orchestration software platform originally developed by Netflix.

This is the basic architecture of conductor:
![image](https://github.com/anushkadeshpande/conductor/assets/53345232/c4f92688-2f84-4b6f-8a39-8103ef3cc3d2)


Documentation: https://conductor-oss.github.io/conductor/devguide/architecture/index.html

Good Read:<br />
https://netflixtechblog.com/netflix-conductor-a-microservices-orchestrator-2e8d4771bf40


Basically, we can define tasks, and multiple `tasks` can be connected in a `workflow`


<hr>

### Setup:

Netflix Conductor Server is a Spring Boot application packaged as JAR file. It will run with embedded tomcat server on port 8080.

#### Server

1. Download `conductor-server-3.3.4-boot.jar` from from <a href="https://repo1.maven.org/maven2/com/netflix/conductor/conductor-server/3.3.4/">Maven Repository</a>
2. Run the conductor server
```sh
java -jar conductor-server-3.3.4-boot.jar
```

Swagger UI of the Conductor server can be accessed via:<br>
http://localhost:8080/swagger-ui/index.html?configUrl=%2Fapi-docs%2Fswagger-config


#### UI

1. Clone this <a href="https://github.com/Netflix/conductor">GitHub Repo</a>
2. Navigate to `conductor-main/ui ` directory and run
```
yarn install
```

> Note: If you don't have yarn installed, you can install it using `npm install --global yarn`

3. To start the frontend application, run
```
yarn run start
```

The web application can be accessed via localhost:5000
