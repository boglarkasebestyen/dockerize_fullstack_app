# FROM node:slim

# # Step 3.1 - Add working directory
# LABEL student student

# # Step 3.2 - Copy npm dependencies
# WORKDIR /src

# # Step 3.3 - Install dependencies
# COPY package.json /src/package.json

# # Copy app source code
# COPY index.js /src/index.js

# RUN npm install

# #Expose port and start the application

# EXPOSE 3000

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
EXPOSE 3000
CMD ["npm", "start"]


