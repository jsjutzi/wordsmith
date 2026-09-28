FROM ubuntu:22.04

WORKDIR /app

COPY pom.xml ./
COPY src ./src

RUN apt-get update && apt-get install -y maven
RUN mvn -B verify

USER nobody
EXPOSE 8080

CMD ["java", "-Xmx8m", "-Xms8m", "-jar", "target/words.jar"]
# CMD exec java -Xmx8m -Xms8m -jar target/words.jar
# The above line will execute the compiled java file
