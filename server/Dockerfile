# FROM node:slim

# # Step 4.1 - Add container working directory
# LABEL student student

# # Step 4.2 - Copy npm dependencies
# WORKDIR /app

# # Step 4.3 - Install dependencies
# COPY package.json /app/package.json

# # Copy app source code
# COPY server.js /app/server.js

# RUN npm install

# #Expose port and start application

# EXPOSE 8080

# CMD ["npm", "start"]


FROM node:slim

# Step 1 - Add container working directory
WORKDIR /app
# Step 2 - Copy npm dependencies
COPY package*.json ./
# Step 3 - Install dependencies
RUN npm install
# Copy app source code
COPY . .

#Expose port and start application
EXPOSE 8080
CMD [ "npm", "start" ]