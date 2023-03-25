# Use an official Node.js runtime as a parent image
FROM node:18

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose port 3000 for the application
EXPOSE 3000

# Start the application
CMD [ "npm", "run", "start" ]

#docker build -t my-nest-app .
#docker run -p 3000:3000 my-nest-app