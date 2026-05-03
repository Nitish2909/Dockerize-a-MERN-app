#Base Image
FROM node:22

#Set Working Directory
WORKDIR /app

# copy package.json and package-lock.json (copy all dependencies)
COPY package*.json ./

# Install Dependencies
RUN npm install

# copy the rest of the application code 
COPY . .

# Expose the port the app runs on
EXPOSE 5173

# Start the application
CMD ["npm", "run", "dev"]

