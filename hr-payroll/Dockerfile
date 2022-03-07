FROM openjdk:11
RUN mkdir /hr-payroll-run
WORKDIR /hr-payroll-run
COPY ./target/hr-payroll-0.0.1.jar .
CMD ["java", "-jar", "hr-payroll-0.0.1.jar"]