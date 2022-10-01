FROM node:9.9.0-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install npm@5.6.0
RUN rm -rf /usr/local/lib/node_modules/npm
RUN mv node_modules/npm /usr/local/lib/node_modules/npm

COPY . .

EXPOSE 8081
CMD [ "node", "index.js" ]