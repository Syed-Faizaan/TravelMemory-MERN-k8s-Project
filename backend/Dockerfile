FROM node:18

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json from backend/
COPY backend/package*.json ./

# Install dependencies
RUN npm install

# Copy everything from backend/
COPY backend/ ./

# Expose the application port
EXPOSE  3001

# Start the application
CMD ["node", "index.js"]