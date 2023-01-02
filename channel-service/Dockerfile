#FROM maven:3.8-jdk-11
## Copy local code to the container image.
#WORKDIR /app
#COPY pom.xml .
#COPY src ./src
#RUN mvn package -DskipTests=true




FROM openjdk:11
COPY target/channel-service-*.jar  /demo.jar
EXPOSE 8788
# Run the web service on container startup.
CMD java -jar /demo.jar
