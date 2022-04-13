FROM node:14

WORKDIR /application

COPY package.json /application

RUN npm install

COPY . /application

EXPOSE 3000

CMD ["node", "server.js"]
