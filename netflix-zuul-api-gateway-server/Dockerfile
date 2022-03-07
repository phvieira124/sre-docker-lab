FROM openjdk:11
RUN mkdir /api-gatway-run
WORKDIR /api-gatway-run
COPY ./target/netflix-zuul-api-gateway-server-0.0.1.jar .
CMD ["java", "-jar", "netflix-zuul-api-gateway-server-0.0.1.jar"]