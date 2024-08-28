FROM openjdk:24-slim-bullseye
EXPOSE 8080
ADD target/rest-demo.jar rest-demo.jar
ENTRYPOINT ["java","-jar","/rest-demo.jar"]