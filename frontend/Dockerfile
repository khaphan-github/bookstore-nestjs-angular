# Use a Node.js base image
FROM node:18

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Build the Angular application
RUN npm run build

# Expose port 3000 (or the port your application runs on)
EXPOSE 3000

# Start the application
CMD ["npm", "start"]