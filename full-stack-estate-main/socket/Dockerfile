# Use a Node.js base image
FROM node:18

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the WebSocket server port (e.g., 5000)
EXPOSE 5000

# Start the WebSocket server
CMD ["node", "app.js"]
