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
