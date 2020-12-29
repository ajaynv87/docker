# Selecting the base image
FROM node:alpine


WORKDIR /usr/app

# copying over the index.js and package.json to the container
COPY ./ ./

# installing modules
RUN npm install

# Specifiying default command to run
CMD ["npm", "start"]