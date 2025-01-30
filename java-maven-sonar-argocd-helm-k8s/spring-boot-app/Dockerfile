# Use Java 17 base image from Eclipse Adoptium
FROM eclipse-temurin:17-jre-alpine

# Define the artifact path (make sure the artifact exists in the 'target' directory)
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy the artifact (JAR file) into the container
COPY ${artifact} app.jar

# Run the JAR file
ENTRYPOINT ["java", "-jar", "app.jar"]
