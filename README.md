# grafana-ha-poc
HA Setup for Grafana with Postgres

# Overview
This Docker Compose file spins up a highly available Grafana setup with two Grafana nodes, 2 PostgreSQL database nodes with repmgr (primary and standby), Nginx reverse proxy to load balance between the Grafana instances and HAProxy to load balance between the PostgresQL instances
It uses Docker volumes for persistent data storage and creates a custom network for inter-service communication.

### Pre-requisites:
- docker
- docker-compose


### Deploy Instructions:
```bash
git clone https://github.com/ppresley/grafana-ha-poc.git
cd grafana-ha-poc
docker compose up -d
```

Go to [localhost:8080](http://localhost:8080) on your browser.
\
\
Initial grafana sign in details:
|Username|Password|
|--------|:------:|
|admin   | admin  |
