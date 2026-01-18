FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

# Expose the port your backend runs on (usually 5000 or 8000)
EXPOSE 5000

# Start the backend server
CMD ["npm", "start"]