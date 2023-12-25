# Use the official Maven image as a base image
FROM maven:3.8-openjdk-17 AS build

# Set the working directory
WORKDIR /usr/src/app

# Copy the POM file and download dependencies
COPY pom.xml .
RUN mvn dependency:go-offline -B

# Copy the application source code
COPY src src

# Build the application
RUN mvn package -DskipTests

# Use OpenJDK as a base image
FROM openjdk:17

# Set the working directory
WORKDIR /usr/src/app

# Copy the JAR file from the build stage
COPY --from=build /usr/src/app/target/sms-backend-0.0.1-SNAPSHOT.jar sms-backend.jar

# Expose the port the app runs on
EXPOSE 8080

# Command to run the application
CMD ["java", "-jar", "sms-backend.jar"]
