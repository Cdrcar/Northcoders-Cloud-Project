# Use an official Node.js runtime as a parent image
FROM node:14.16.1-alpine3.13 AS base

# Set the working directory to /app
WORKDIR /app
# Copy the package.json and package-lock.json files
COPY ["package.json", "package-lock.json*", "./"]
# Install dependencies
RUN npm install 
# Copy the rest of the application code
COPY . .

# for lint



# for build

FROM base as builder

WORKDIR /app


# Build the application
RUN npm run build

# Expose port 8080
EXPOSE 5173

# Run the application
CMD ["npm", "start"]