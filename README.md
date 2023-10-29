# Getting started
## Prerequisites
- Java 17
- A running Keycloak instance
- A running Postgresql server

## Configuration
- Add a properties file to the project root. This file should have the name ".env.properties"
  - The .env.properties.example has a set of default values. Type `mv .env.properties.example .env.properties` in the terminal if you want to use this default value
  -- When using the default values it is mandatory to update the GITPOD_FRONTEND_URL to your own frontend url. This can be found by starting the frontend gitpod and then look at the 'Ports' tab. The URL that contains 4200 should be used as the value

## Gitpod configuration
- Set the front-end URL in the .env.properties file (you can find this in the front-end Gitpod under the 'Ports' tab for port 4200)

## Starting up
- Run the following command from a terminal in the project root: ```./gradlew bootrun``` or go to the Gradle tab on the left side (elephant icon) and run the bootRun task in the application folder
- Make sure that port 8080 is made public after starting the back-end, you can check this under the 'Ports' tab by making sure the lock icon for port 8080 is an open lock

## Supporting containers
The Valtimo backend application requires a Keycloak instance and a database server. When running the application locally, running Keycloak and the database locally as well is recommended. In the [valtimo-docker-compose repository](https://github.com/valtimo-platform/valtimo-docker-compose), Docker compose files are available to support the Valtimo application. This repository includes a guide on which Compose file to use.

# Adding implementation code
