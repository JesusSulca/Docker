FROM alpine:latest

ENV JAVA_HOME="/usr/lib/jvm/default-jvm/"
RUN apk add openjdk11

ENV PATH=$PATH:${JAVA_HOME}/bin

CMD ["jshell"]

COPY target/Ms-User-0.0.1-SNAPSHOT.jar /challenge5.jar

ENTRYPOINT ["java", "-jar", "/challenge5.jar"]

EXPOSE 8084