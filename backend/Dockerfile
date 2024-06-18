# Use the official Node.js image with a specified version as base
FROM node:14

# Set the working directory inside the container
WORKDIR /app/backend

# Copy package.json and package-lock.json to the working directory
COPY backend/package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the backend code to the working directory
COPY backend/ .

# Expose port 5000
EXPOSE 5000

# Command to run the backend server
CMD ["npm", "run", "dev"]
