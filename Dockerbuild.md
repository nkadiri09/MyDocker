## Creating docker image from docker build

    Dockerbuild  #sample docker file
      # getting base image from ubuntu
      FROM ubuntu:latest
      MAINTAINER narendra <nkadiri09@gamil.com>
      RUN apt-get update && apt-get install -y git
      RUN apt-get install -y openjdk-8-jdk
      WORKDIR /usr/local/bin/
      COPY test-program.jar
      CMD ["java", "-jar", "test-program.jar"]
      # CMD ["echo", "Hello World...! from my first docker file"]
      # CMD ["/bin/bash"]
    
    docker build -t <name-of-the-image-you-r-building:version> directory
