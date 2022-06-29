FROM node

WORKDIR /app

COPY package*.json .

RUN npm install

COPY . .

EXPOSE 80

VOLUME ["logs:/app/logs"]
 
VOLUME ["/app/node_modules"]

ENV MONGODB_USERNAME=mongoadmin
ENV MONGODB_PASSWORD=secret

CMD [ "npm", "start" ]