# grafana-ha-poc
HA Setup for Grafana with Postgres

# Overview
This Docker Compose file sets up a highly available Grafana setup with two Grafana instances, a PostgreSQL database, and an Nginx reverse proxy to load balance between the Grafana instances. 
It uses Docker volumes for persistent data storage and a custom network for inter-service communication.

### Pre-requisites:
- docker
- docker-compose

### Deploy Instructions:
```bash
docker compose up -d
```

Go to [localhost:8080](http://localhost:8080) on your browser.
\
\
Initial grafana sign in details:
|Username|Password|
|--------|:------:|
|admin   | admin  |