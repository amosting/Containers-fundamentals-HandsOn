# L05-04

Type the following Docker commands:

## Pull and run a Nginx server

    docker run -d -p 8080:80 --name webserver nginx
- `docker run -d -p <LOCAL_PORT>:<CONTAINER_LISTENER_PORT> --name <RUNNING_INSTANCE_NAME> <CONTAINER_IMAGE_NAME>`
- `-d`: Detached mode
    - The container runs in the background (as a daemon), allowing user to continue using terminal for other commands

## List the running containers

    docker ps

## List the images

    docker images

## Attach to the container

    docker container exec -it  webserver bash  

Exit by typing

    exit

## Stop the container

    docker stop webserver
- `docker STOP <RUNNING_INSTANCE_NAME>`

## Remove the container from memory

    docker rm webserver
- `docker rm <RUNNING_INSTANCE_NAME>`

## Remove the image

    docker rmi nginx
- `docker rmi <CONTAINER_IMAGE_NAME>`