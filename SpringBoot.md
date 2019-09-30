## Building springBoot docker image


    FROM openjdk:8
    ADD target/MySpringBootApp.jar MySpringBootApp.jar
    VOLUME /tmp
    EXPOSE 7085
    ENTRYPOINT ["java","-jar","MySpringBootApp.jar"]
    
    

    FROM openjdk:8-jdk-alpine
    VOLUME /tmp
    ARG JAR_FILE
    COPY ${JAR_FILE} app.jar
    ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
