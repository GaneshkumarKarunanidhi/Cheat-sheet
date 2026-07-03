# Docker :shark: 
Docker is a platform designed to help developers build, share, and run container applications.Developer can focus on the code.
It's enables you to separate your applications from your infrastructure so you can deliver software quickly.

It's gives an guarantee of   `Build Once and Run Anywhere`:stars:.

## Docker Image
Docker images are a lightweight, standalone, executable package of software that includes everything needed to run an application: 
code, runtime, system tools, system libraries and settings.

## Docker Containers 
A container is a runtime instance of a docker image. A container will always run the same, regardless of the infrastructure. 
Containers isolate software from its environment and ensure that it works uniformly despite differences for instance between development and staging.

## Docker commands

| Commands | Description |
| -------- | -------- | 
| **VIEW** 👀 |
|docker ps | Lists all running contains |
|docker ps -a | Lists all contains include stopped |
|docker images| List all local images| 
|docker volumes | List all volumes |
| **INFORMATION** 📝 |
|docker info | Display system-wide information|
|docker container stats | view resource usage stats|
| **RUN AND BUILD** 🚀 |
|docker build -t image_name:tagNo |Build an Image from a Dockerfile |
|docker build -t image_name:tagNo -no-cache |Build an Image from a Dockerfile without the cache |
|docker run --name <container_name>  -p <host_port>:<container_port> -e Key1:Value1 -e Key2:Value2 <image_name> | Create and run a container from an image, with a custom name,port and set environment variables |
|docker run --env-file .env <image_name> | set multiple environment variables using an .env file  |
|docker compose up -d | Create a docker-compose.yml file and run a multiple container and in a Detachable mode |
|docker compose -f <compose_fileName> up -d | If you are maintain a different compose file  then you can choose particular file using an -f parameter |
|docker compose stop | Stop all containers mentioned in compose.yml file |
|docker compose down | Stop and remove all containers mentioned in compose.yml file |
|docker start <container_name> | start the container |
|docker stop <container_name> | stop the container |
| **DEBUG** 🛠️ |
|docker inspect| Inspect docker container it contains config,env variables,Mounts path, Image details, Run Commands,Created details and etc  |
|docker exec -it <container_name> bash | Open a linux/bash file system inside a running container |
|docker cp <container_name>:<file_path> . | Copy files from container |
|docker logs <container_name> or <container-id> | View container application logs |
|docker logs -f <container_name> or <container-id> | View live logs of the container |
|docker logs -f  --tail number <container_name> or <container-id> | Get last logs based on mentioned number and View live logs of the container |
|docker logs <container_name> > outLog.txt; | Export logs from container |
|**DELETE** 🗑️|
|docker rm <container_name> | Delete/Remove an container |
|docker rm -f <container_name> | Force fully Delete/Remove an container |
|docker rmi <image_name>| Delete/Remove an  Image |
|docker image prune | Remove all unused images |
|docker system prune -a | Remove unused container(it's not running),images and volumes |


## Happy Learning :book: :rocket: 💚
