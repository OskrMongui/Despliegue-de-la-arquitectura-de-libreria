# ---- BASE NODE IMAGE ----
FROM node:18

# Create app directory
WORKDIR /usr/src/app

# Copy package.json files
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy all project files
COPY . .

# Expose the port the app uses
EXPOSE 3000

# Start the node server
CMD [ "node", "server.js" ]
