# Base image
FROM eclipse-temurin:17-jdk-alpine

WORKDIR /app

# Copy the jar from target
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Expose service port
EXPOSE 8082

# Run the jar
ENTRYPOINT ["java","-jar","/app.jar"]
