---
title: Docker Cheatsheet
tags:
  - docker
  - devops
  - cheatsheet
date: 2026-03-28
---

Tổng hợp các lệnh Docker thường dùng.

## Images

```bash
# Pull image
docker pull nginx:latest

# List images
docker images

# Build image
docker build -t my-app:1.0 .

# Remove image
docker rmi <image-id>
```

## Containers

```bash
# Run container
docker run -d -p 8080:80 --name my-container nginx

# List running containers
docker ps

# List all containers
docker ps -a

# Stop container
docker stop <container-id>

# Remove container
docker rm <container-id>

# View logs
docker logs <container-id>
```

## Docker Compose

```bash
# Start services
docker-compose up -d

# Stop services
docker-compose down

# View logs
docker-compose logs -f

# Rebuild and start
docker-compose up -d --build
```

## Volume & Network

```bash
# List volumes
docker volume ls

# Create volume
docker volume create my-volume

# List networks
docker network ls
```

## Useful Tips

```bash
# Remove all stopped containers
docker container prune

# Remove unused images
docker image prune -a

# Remove everything
docker system prune -a
```

---

> Xem thêm: [[notes]]
