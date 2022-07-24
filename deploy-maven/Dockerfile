FROM ubuntu:18.04

RUN apt-get update -y
RUN apt-get install -y git openjdk-17-jre openjdk-17-jdk maven
RUN apt-get install -y default-jre default-jdk maven curl git
RUN export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64/
EXPOSE 8080
RUN git clone https://gitlab.com/Sirenitix/spring-boot-docker.git
WORKDIR /spring-boot-docker/
CMD ["./mvnw", "spring-boot:run"]

