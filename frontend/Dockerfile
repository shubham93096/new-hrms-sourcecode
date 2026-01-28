# Use official Node.js image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json first to leverage caching
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the project files
COPY . .

# Expose port 4200 for container communication
EXPOSE 4200

# Run Angular development server on all interfaces
CMD ["npx", "ng", "serve", "--host", "0.0.0.0", "--port", "4200"]
