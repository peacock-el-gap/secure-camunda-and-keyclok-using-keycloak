# Securing Camunda & Keycloak using Keycloak

<div style="color: red; font-size: xx-large">
Work in progress
</div>

## Infrastructure
Run PostgreSQL + Keycloak + Camunda
```shell
# This script has to be executed in project root
docker-compose -f ./postgresql-and-camunda-and-keycloak/docker-compose.yaml up -d
```
Note, that on first run PostgreSQL initialization for Camunda schema / tables can last to long and Camunda will not be able to start properly.
Wait until PostgreSQL initialization ends, stop the service and run it again. It should start without any problem. 

Stop PostgreSQL + Keycloak + Camunda
```shell
# This script has to be executed in project root
docker-compose -f ./postgresql-and-camunda-and-keycloak/docker-compose.yaml down
```

