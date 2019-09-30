# Installing Jenkins in Docker:

      Docker pull Jenkins

To run docker jenkins docker image as container:

      Docker run -p 8080:8080 -p 50000:50000 jenkins

To run commands inside the docker container:

      Docker run -it <docker-containser-name>

      Docker inspect <image-name> provides the full information on docker image.

To build our own docker image:

      Docker build -f  <docekr-file-path> -t <name of the docker image u want to create.>
