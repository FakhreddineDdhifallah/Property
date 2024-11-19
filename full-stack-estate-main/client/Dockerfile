# Use a lightweight Node.js image
FROM node:18 AS build

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Build the application
RUN npm run build

# Use an NGINX image to serve the built files
FROM nginx:alpine

# Copy built files from the previous stage
COPY --from=build /usr/src/app/dist /usr/share/nginx/html

# Expose the default NGINX port
EXPOSE 80

# Start NGINX
CMD ["nginx", "-g", "daemon off;"]
