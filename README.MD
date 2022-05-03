# Basic Commands

- pull image from registry

`docker pull nginx`

- list every pulled images

`docker images` same as `docker image ls`

- run container in detached mode (-d) and binding localhost:8080 to container:80 (-p)

`docker run -d nginx:latest -p 8080:80`

- list running containers

`docker ps` same as `docker container ls`

- stop container with given name or id

`docker stop 7f42b5e7` or `docker stop alfredo-salmon`
