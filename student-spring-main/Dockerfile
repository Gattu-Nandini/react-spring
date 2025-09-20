# Use OpenJDK
FROM container-registry.oracle.com/java/jdk:23


WORKDIR /app

COPY target/*.jar app.jar

EXPOSE 8080

# Pass Render's $PORT to Spring Boot

CMD ["sh", "-c", "java -Dserver.port=$PORT -jar app.jar"]
