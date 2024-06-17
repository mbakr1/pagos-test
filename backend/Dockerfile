FROM node:14

WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

COPY . .

# Expose the port the app runs on
EXPOSE 3000

# Define environment variables (DB_USERNAME and DB_PASSWORD will be provided by Docker Compose)
ENV DB_USERNAME=${DB_USERNAME}
ENV DB_PASSWORD=${DB_PASSWORD}

# Start the application
CMD ["node", "app.js"]
