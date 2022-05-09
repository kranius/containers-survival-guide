# Basic Docker Commands


## Useful links

[Official reference](https://docs.docker.com/reference/)

[file/process duality](https://iximiuz.com/en/posts/containers-101-container-mgmt-commands/)

[dockerfile](https://docs.docker.com/engine/reference/builder/)

- pull image from registry

`docker pull nginx`

- list every pulled images

`docker images` same as `docker image ls`

- run container in detached mode (-d) and bind localhost:8080 to container:80 (-p)

`docker run -d -p 8080:80 nginx:latest`

- list running containers

`docker ps` same as `docker container ls`

- stop container with given name or id

`docker stop 7f42b5e73254` or `docker stop alfredo-salmon`

- delete container

`docker rm 7f42b5e73254`

- run container and give it name

`docker run --name website -d -p 8080:80 nginx:latest`

- start/stop

`docker start website`

`docker stop website`

- run container with volume

`docker run -v /my/local/html/files:/usr/share/nginx/html:ro --name website -d -p 8080:80 nginx:latest`

- start bash inside container

`docker exec -it website bash`


# Basic kubernetes commands
