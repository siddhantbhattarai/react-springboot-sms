# Use an official Node runtime with Alpine Linux as a parent image
FROM node:18-alpine

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the local code to the container
COPY . .

# Build the application
RUN npm run build

# Expose the port that the app will run on
EXPOSE 3000

# Run the command to start your app
CMD ["npm", "start"]
