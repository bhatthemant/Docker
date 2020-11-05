# # Choose the base image
# FROM node:latest
# # Set the 'app' folder as working dir inside container; this also creates the app folder if it doesn't exists
# WORKDIR /app
# # Copy everything from current folder to current folder 'app'
# ADD . .
# # Run the command to install all dependcies in the pacakge.json
# RUN npm install
# # Command to run the node api
# CMD node index.js


FROM node:alpine

WORKDIR /app

ADD package*.json /.

RUN npm install

ADD . .

CMD node index.js