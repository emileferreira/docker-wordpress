# Docker WordPress

A Docker Compose file to orchestrate WordPress deployment.

## Requirements

- Docker Engine 25.0.2+
- Docker Compose 2.24.5+

## Usage

Pull the Docker images and launch the containers. WordPress will be available at [localhost:10080](http://localhost:10080). The port number can be changed in [docker-compose.yaml](docker-compose.yaml).

```Bash
docker-compose up -d
```

## Updating

WordPress updates initiated from the WordPress dashboard will not persist container reboots. Instead, the WordPress Docker image should be updated as follows.

```Bash
docker-compose down
docker pull wordpress
docker-compose up -d
```
