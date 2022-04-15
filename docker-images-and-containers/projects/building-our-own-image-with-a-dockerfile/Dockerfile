FROM node:12

WORKDIR /application

COPY package.json /application

RUN npm install

COPY . /application

EXPOSE 80

CMD ["node", "server.js"]
