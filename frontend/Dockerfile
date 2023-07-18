# Use an official Node.js runtime as the base image with version 18.15.0
FROM node:18.15.0-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install project dependencies
RUN npm install

# Copy the entire project to the working directory
COPY . .

# Build the React app
RUN npm run build

# Specify the command to run your app
CMD [ "npm", "start" ]
