# Image to create the container
FROM node

# set the working directory to app folder
WORKDIR /app 

# copy the package.json file to the container
COPY package.json /app

# install dependencies
RUN npm install

# copy all files from the root or the project to the current
# working directory of the container
COPY . /app

# expose container to outside in port 3000
EXPOSE 3000

# to run command in the container uses the CMD directive
# if use the Run directive its run on the image
CMD [ "node", "server.js" ]