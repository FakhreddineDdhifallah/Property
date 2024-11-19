# 1. Use the official Node.js image as the base
FROM node:16

# 2. Set the working directory inside the container
WORKDIR /app

# 3. Copy package.json and package-lock.json files
COPY package*.json ./

# 4. Install Node.js dependencies
RUN npm install

# 5. Copy the rest of the backend files into the container
COPY . .

# 6. Expose the port your backend uses (e.g., 8080)
EXPOSE 8080

# 7. Command to run your backend
CMD ["npm", "start"]
