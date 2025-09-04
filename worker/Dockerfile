FROM joshua122/worker:v2 AS build
WORKDIR /code
COPY . . 
RUN mvn package -Dskiptests

FROM openjdk:8-jre-alpine
WORKDIR /run
COPY --from=build /code/target/worker-jar-with-dependencies.jar worker.jar
CMD ["java", "-jar", "worker.jar"]
