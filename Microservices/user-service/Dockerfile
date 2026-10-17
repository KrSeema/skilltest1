
# Use an official Node.js base image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package information
COPY package*.json ./

# Install application dependencies
RUN npm install --omit=dev

# Copy application source code
COPY . .

# Document the port used by the application
EXPOSE 3000

# Start the User Service
CMD ["node", "app.js"]