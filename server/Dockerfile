# Use an official Node runtime as the base image
FROM node:20-slim

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Bundle app source inside the Docker image
COPY . .

# Expose port 3000 to the outside world
EXPOSE 3001

# Define the command to run your app using CMD which defines your runtime
CMD ["npm","start"]
