# Simple Docker Commands.

### Docker practice Website: https://labs.play-with-docker.com/

      Basic
      : docker version
      : docker -v
      : docker info
      : docker --help
      : docker login
      ————————————
      Images
      : docker images
      : docker pull
      : docker rmi
      ————————————
      Containers
      : docker ps
      : docker run
      : docker start
      : docker stop
      ————————————
      System
      : docker stats
      : docker system df
      : docker system prune


## Docker Commands:

Pulling docker image:

	Docker image pull <Docker-imange-name>

Running docker container:

	Docker container -p <public-port>:<docker-port>
		Run container as Demond -d
			Docker container -d -p <public-port>:<docker-port>

List all docker container List:

	Docker container ls


Docker Logs

	Docker container logs <container-name> container log
	Docker container -f logs <container-name> monitor a log to follow log.


-it : interactive terminal.	

To run various commands inside the docker container.

	Docker container exec -it <container-name-id> bash


## Installing Jenkins in Docker:

Docker pull Jenkins

To run docker jenkins docker image as container:

Docker run -p 8080:8080 -p 50000:50000 jenkins

To run commands inside the docker container:

Docker run -it <docker-containser-name>

Docker inspect <image-name> provides the full information on docker image.

To build our own docker image:
Docker build -f  <docekr-file-path> -t <name of the docker image u want to create.>
