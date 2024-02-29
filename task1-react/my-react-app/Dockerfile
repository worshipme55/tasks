# Use an official Node.js image as the base image
FROM node:19

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install project dependencies
RUN npm install

# Copy the entire project to the working directory
COPY . .

# Expose the port that the app will run on
EXPOSE 5173

# Define the command to run your app
CMD ["npm", "run", "dev"]
