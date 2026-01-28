# Use official lightweight Python image
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy all files into container
COPY . .

# Expose port 8080 for container communication
EXPOSE 8080

# Start simple HTTP server on container startup
CMD ["python3", "-m", "http.server", "8080"]
