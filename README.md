# Keycloak Deploy Kubernetes

## 1. Deploy using Kubernetes and external database


`kubectl apply -f keycloak-deployment.yaml`

## 2. Deploy using only docker
`docker run -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin  -p 8080:8080 quay.io/keycloak/keycloak:22.0.0 start-dev`



## 2. Deploy using Docker compose

### Create Docker database and Keycloak
In this scenareo, using:
 * Postgresql
 * Keycloak version: 22.0.0

 Execture follow comand for running docker compose:
`docker-compose up -d`