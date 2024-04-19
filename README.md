# compose
Examples of docker compose files. 

I created this repo because it is always difficult to find such simple files.

The only non default configuration here is the network, as I prefer to create customized subnets to avoid conflict with default ip routes.

I will add new files eventually. 

# Getting Started

Follow this documentation to run the components within Docker.

## Requirements

- Docker Engine (if you are using Docker Desktop, it requires version 4.22+)
- Docker Compose 2.20.3+

## Run

Clone this repository and run the application:

Starting postgres database, its volume, and customized network:
```bash
docker compose -f postgres.yml up -d
```

Starting redis database, not persistent, and customized network:
```bash
docker compose -f redis.yml up -d
```
