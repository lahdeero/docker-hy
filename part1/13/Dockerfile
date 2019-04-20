FROM openjdk:12.0.1-jdk
CMD mkdir /usr/src
CMD mkdir /usr/src/spring-example-project
COPY ./spring-example-project /usr/src/spring-example-project
WORKDIR /usr/src/spring-example-project
RUN /usr/src/spring-example-project/mvnw package
RUN ls -la /usr/src/spring-example-project
ENTRYPOINT java -jar /usr/src/spring-example-project/target/docker-example-1.1.3.jar

