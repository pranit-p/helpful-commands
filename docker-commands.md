
> docker pull <image_name>(ubuntu) 

> docker run <image_name>(ubuntu)

> docker ps (list of running containers)

> docker ps -a (list of running and stopped containers)

> docker run -it <image_name>(ubuntu) 
(go inside the ubuntu container (open in interactive mode))

> docker start -i <container_id> 

> docker exec -it -u pranit container_name bash 
(login to the container as a pranit user)

> docker exec	(for executing command inside the container )

> docker build -t <image_name_that_you_want> .

> docker images

> docker run -it <image_name> <bash/sh> it will open file directory of image

> docker history <image_name> (to see history of image)

> docker image prune  (removing unwanted images )

> docker image rm <image_id/image_name> 
(remove docker image from the system)

> docker build -t <image_name>:<tag_value> . (change tag of image)

> docker image tag <image_name>:<new_tag> <image_name>:<new_tag>
(change tag of image)

> docker login 

> docker push <image_name>:<tag>  

> docker image save -o <name_file_in_tar_extension/demo.tar> <image>:version 

> docker image load -i <tar_file>

> docker run <image_name> (running container with image)

> docker run -d <image_name> (running container in background)

> docker ps (show list of the running container)

> docker log <image_name> (it will print logs of container)

> docker run -d -p <host_port>:<container_port> —name <container_name> <image_name>
	(connecting the host port and container port )

> docker exec <container_name> <linux_command
Ex: docker exec c1 ls

> docker exec -it <container_name> <sh/bash>
	Ex: docker exec -it c1 sh

> docker volume create <volume_name_anything_you_want>

> docker volume inspect <volume_name> 
	(It will give us details of the volume)

> docker run -d -p <host_port>:<container_port> -v <volume_name>:<folder_in_container> <image_name>
	(it will create volume and attach to the container)

> docker copy <source> <destination>
	Ex:  docker copy 0135575:app/log.txt . 

> docker run -d -p <host_port>:<container_port> -v $(pwd):<container_directory> <image_name>


Example: 
	docker run -d -p 5001:3000 -v $(pwd):/app demo-angular-app


> docker container rm -f $(docker container ls -aq)

> docker container rm -f $(docker container ls -q)

> docker image rm -f $(docker image ls -a q)



> docker-compose build (it will build all container register in compose)

> docker-compose up -d (it will run all container register in compose) 

> docker-compose down 

> docker-compose ps


> docker network ls

> docker exec -it -u root <container_id> sh  (login to container as root user)

> docker-compose logs



> docker-machine ls



> docker-machine create --driver amazonec2 <server_name>
