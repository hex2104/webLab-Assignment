# Use the official Node.js image with a specified version as base
FROM node:14

# Set the working directory inside the container
WORKDIR /app/frontend

# Copy package.json and package-lock.json to the working directory
COPY frontend/package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the frontend code to the working directory
COPY frontend/ .

# Expose port 3000 (assuming your React app runs on this port)
EXPOSE 3000

# Command to run the frontend server
CMD ["npm", "start"]
