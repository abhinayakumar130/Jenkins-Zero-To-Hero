# Use a Java 17 base image
FROM adoptopenjdk:17-jre-alpine

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java", "-jar", "app.jar"]
