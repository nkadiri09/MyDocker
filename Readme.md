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
