FROM openjdk:11
RUN mkdir /hr-worker-run
WORKDIR /hr-worker-run
COPY ./target/hr-worker-0.0.1.jar .
CMD ["java", "-jar", "hr-worker-0.0.1.jar"]