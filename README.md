# Containerization

This project collects my understanding and notes to containerization relevant knowledge.

# 7 Docker Commands You Must Remember

<code>[docker ps -a](https://docs.docker.com/reference/cli/docker/container/ls/)</code>: list containers

<code>[docker run {image} --name {name}](https://docs.docker.com/reference/cli/docker/container/run/)</code>: run containers, same with <code>docker create</code> + <code>docker start</code>

<code>[docker system prune -a](https://docs.docker.com/reference/cli/docker/system/prune/)</code>: remove all stopped containers, all networks not used by at least one container, all dangling images, unused build cache

<code>[docker build](https://docs.docker.com/reference/cli/docker/build-legacy/)</code>: build an image from Dockerfile

<code>[docker stop {container}](https://docs.docker.com/reference/cli/docker/container/stop/)</code>: stop a container

<code>[docker rm {container}](https://docs.docker.com/reference/cli/docker/container/rm/)</code>: remove a container

<code>[docker exec -it {container} /bin/sh](https://docs.docker.com/reference/cli/docker/container/exec/)</code>: execute a command in a running container

# How to use Dockerfile.dev
Dockerfile.dev and docker-compose.yml is used during frontend development stage as a containerization solution.
To use apply them to frontend development, you can run 3 commands,
```
docker compose build web # Build an image
docker compose down web # Stop web
docker compose up web # Run the latest image
```

```
To get more information about how image is built, refer to https://stackoverflow.com/questions/35774714/how-to-cache-the-run-npm-install-instruction-when-docker-build-a-dockerfile
```
