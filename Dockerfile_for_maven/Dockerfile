FROM maven:3.8.6-openjdk-18 AS build
COPY src /home/app/src
COPY pom.xml /home/app
RUN mvn -f /home/app/pom.xml clean package

FROM openjdk:8-jdk-alpine
COPY --from=build /home/app/target/spring-boot-app-1.0-SNAPSHOT.jar /usr/local/lib/spring-boot-app.jar 
EXPOSE 8080
ENTRYPOINT ["java","-jar","/usr/local/lib/spring-boot-app.jar", ""]