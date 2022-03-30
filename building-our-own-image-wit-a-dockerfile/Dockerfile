# Using Node.js image
FROM node 

# Defining working directory
WORKDIR /application


COPY . /application

RUN echo 'installing dependencies'

RUN npm install 

EXPOSE 80

CMD ["node", "server.js"]

# docker run -p 3000:80 <id>