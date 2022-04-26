FROM node:14

WORKDIR /application

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=leonardo

ENV MONGODB_PASSWORD=1234

CMD ["npm", "start"]