# Use the official Node.js runtime as a parent image
FROM node:14

# Set the working directory in container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN yarn install

# Copy the content of the local src directory to the working directory
COPY . .

# Declare the port the app runs on
EXPOSE 3000

# Command to run the app
CMD [ "yarn", "start" ]
