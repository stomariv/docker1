FROM openjdk:18.0.2.1-jdk
RUN microdnf install git
RUN git clone https://github.com/spring-projects/spring-petclinic.git
WORKDIR /spring-petclinic/
RUN ./mvnw package
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "/spring-petclinic/target/spring-petclinic-2.7.3.jar"]