FROM openjdk:11
RUN mkdir /eureka-server
WORKDIR /eureka-server
EXPOSE 8761
COPY ./target/hr-eureka-server-0.0.1.jar .
CMD ["java", "-jar", "hr-eureka-server-0.0.1.jar"]