# You can change this base image to anything else
# But make sure to use the correct version of Java
# FROM adoptopenjdk/openjdk11:alpine-jre

# # Simply the artifact path
# ARG artifact=target/spring-boot-web.jar
# #ARG artifact=target/

# WORKDIR /opt/app

# COPY ${artifact} app.jar

# # This should not be changed
# ENTRYPOINT ["java","-jar","app.jar"]

FROM lolhens/baseimage-openjre
ADD target/springbootApp.jar springbootApp.jar
EXPOSE 80
ENTRYPOINT ["java", "-jar", "springbootApp.jar"]

