FROM openjdk:17-jdk-slim
WORKDIR /app
COPY target/users-api.jar users-api.jar
EXPOSE 8081
CMD ["java", "-jar", "users-api.jar"]
