FROM openjdk:11-jre-slim
RUN apt-get update && apt-get install -y maven

COPY . app/
WORKDIR /app

COPY target/Code.jar app.jar
CMD ["java", "-jar", "app.jar"]