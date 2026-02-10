# Use official Node.js LTS image
FROM node:20-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package files
COPY package*.json ./

# Install dependencies with audit fix
RUN npm install --production && npm audit fix

# Copy source code
COPY . .

# Remove sensitive files
RUN rm -f encryptionkeys/jwt.key encryptionkeys/jwt.pub

# Set non-root user
USER node

# Expose the application port
EXPOSE 3000

# Start the app
CMD ["npm", "start"]

