# Use a lightweight Node.js image
FROM node:20-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the frontend source code
COPY . .

# Vite usually runs on port 5173
EXPOSE 5173

# Run the frontend (Vite requires --host to be accessible from outside the container)
CMD ["npm", "run", "dev", "--", "--host"]