FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm ci --omit=dev

# Copy backend source code
COPY . .

# Backend listens on port 3000
EXPOSE 3000

# Start the application
CMD ["npm", "start"]