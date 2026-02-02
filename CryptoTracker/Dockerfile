# Use Java 17
FROM eclipse-temurin:17-jdk

# Set working directory
WORKDIR /app

# Copy project files
COPY . .

# Build the application
RUN ./mvnw clean package -DskipTests

# Expose port (Render uses PORT env variable)
EXPOSE 8080

# Run the app
CMD ["java", "-jar", "target/*.jar"]
