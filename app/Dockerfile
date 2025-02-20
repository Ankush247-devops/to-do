# Use a lightweight Node.js base image
FROM node:18-alpine

# Set working directory inside the container
WORKDIR /app

# Copy package files and install dependencies
COPY package.json package-lock.json ./
RUN npm install 

# Copy the application source code
COPY . .

# Expose the application's port (change if necessary)
EXPOSE 5000

# Start the Node.js application
CMD ["node", "server.js"]
