# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM adoptopenjdk/openjdk11:armv7l-ubuntu-jre-11.0.23_9

# Simply the artifact path
ARG artifact=target/spring-boot-web-subbu.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
