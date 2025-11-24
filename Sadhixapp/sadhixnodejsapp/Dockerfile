# Use a lightweight Node.js base image
FROM node:alpine

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of your application files
COPY . .

# Expose the port your app listens on
EXPOSE 3000

# Start the application
CMD ["node", "index.js"]
