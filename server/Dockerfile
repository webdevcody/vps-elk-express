# Use an official Node.js runtime as the base image
FROM node:18

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install application dependencies
RUN npm install

# Copy the application code into the container
COPY . .

# Expose the port your Express app is listening on (e.g., 3000)
EXPOSE 3000

# Define the command to start your Express application
CMD [ "node", "index.js" ]