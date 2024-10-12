# Use an official Node.js runtime as a parent image
FROM node:20

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json files to install dependencies
COPY package*.json /usr/src/app

# Install dependencies for the backend
RUN npm install 20

# Copy the entire application source code to the container
COPY . .

# Expose the port that your app runs on
EXPOSE 3001

# Set environment to production (or use a different value based on your needs)
ENV NODE_ENV=production

# Command to start your application
CMD ["npm", "start"]

