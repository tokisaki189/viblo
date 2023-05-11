# Use an official Node.js base image
FROM node:18

# Set the working directory in the Docker image
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install Node.js dependencies
RUN npm ci

# Copy the rest of the application files to the working directory
COPY . .

# Expose the port that the application will run on
EXPOSE 3000

# Start the Node.js application
CMD ["node", "server.js"]

# Tag the image with latest
