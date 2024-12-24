# Use an official OpenJDK 21 Alpine-based image to run the application
FROM openjdk:21-jdk-slim

# Set working directory
WORKDIR /app

# Copy the pre-built JAR file to the container
COPY target/order-service-0.0.1-SNAPSHOT.jar ./order-service.jar

# Expose the port for the service
EXPOSE 8083

# Command to run the application
CMD java -jar order-service.jar