FROM node:14

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

RUN npm install 

# Copy the rest of the application code
COPY . .

# Expose the port that the server listens on
EXPOSE 3001

# Start the server
CMD ["npm", "start"]

