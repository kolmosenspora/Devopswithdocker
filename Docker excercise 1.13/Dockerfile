FROM openjdk:8
COPY spring-example-project-master spring-example-project-master
WORKDIR /spring-example-project-master
RUN ./mvnw package
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
EXPOSE 8080