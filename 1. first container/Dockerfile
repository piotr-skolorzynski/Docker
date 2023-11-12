#means we want node in version 14 inside container
FROM node:14

#create directory app
WORKDIR /app

#copy package.json file to our app directory
COPY package.json .

#then run npm install command to install all dependecies from package.json
RUN npm install

#copy the rest of code
COPY . .

#create a web server listening for incoming requests on port 3000
EXPOSE 3000

#execute app.mjs file with node command
CMD [ "node", "app.mjs" ]