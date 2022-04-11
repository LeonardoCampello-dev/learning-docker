# Using Node.js image
FROM node 

# Defining working directory
WORKDIR /application

COPY package.json /application

RUN echo 'installing dependencies'

RUN npm install

COPY . /application

EXPOSE 80

CMD ["node", "server.js"]

# docker run -p 3000:80 <id>