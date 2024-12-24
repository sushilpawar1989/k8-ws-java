# Use an official OpenJDK 21 Alpine-based image to run the application
FROM openjdk:21-jdk-slim

# Set working directory
WORKDIR /app

# Copy the pre-built JAR file to the container
COPY target/inventory-service-0.0.1-SNAPSHOT.jar ./inventory-service.jar

# Expose the port for the service
EXPOSE 8082

# Set environment variables with default values (which can be overridden)
ENV ESPRESSO_SHOT_QUANTITY=5 \
    MILK_QUANTITY=10 \
    HOT_WATER_QUANTITY=20 \
    MILK_FOAM_QUANTITY=15 \
    INVENTORY_URL=http://localhost:8082

# Command to run the application
CMD java -jar inventory-service.jar