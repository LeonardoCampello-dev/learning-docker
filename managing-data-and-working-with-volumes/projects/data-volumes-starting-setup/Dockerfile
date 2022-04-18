FROM node:14

WORKDIR /application

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

VOLUME ["/application/feedback"]

CMD ["node", "server.js"]