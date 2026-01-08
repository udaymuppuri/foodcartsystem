# Use Node.js image
FROM node:22

# Set working directory
WORKDIR /app

# Copy package files first (for caching)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy rest of the frontend code
COPY . .

# Expose Vite default port
EXPOSE 5173

# Start Vite dev server
CMD ["npm", "run", "dev"]
