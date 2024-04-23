# Docker WordPress

A Docker Compose file to orchestrate WordPress deployment.

## Setup

```Bash
docker-compose up -d
```

## Updating

WordPress updates initiated from the WordPress dashboard will not persist container restarts. Instead, the WordPress Docker image need to be updated.

```Bash
docker-compose down
docker pull wordpress
docker-compose up -d
```
