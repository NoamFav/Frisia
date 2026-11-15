# Use an official OpenJDK runtime
FROM openjdk:17-jdk-slim

# Set working directory
WORKDIR /app

# Copy the packaged jar into the container
COPY target/server-1.0-SNAPSHOT.jar /app/server.jar

# Expose port (matches Fly.io requirements)
EXPOSE 9000

# Run the application
CMD ["java", "-jar", "server.jar"]
