# Docker WordPress

A Docker Compose file to orchestrate WordPress deployment.

## Setup

Pull the Docker images and launch the containers.

```Bash
docker-compose up -d
```

## Update

WordPress updates initiated from the WordPress dashboard will not persist container reboots. Instead, the WordPress Docker image should be updated as follows.

```Bash
docker-compose down
docker pull wordpress
docker-compose up -d
```
