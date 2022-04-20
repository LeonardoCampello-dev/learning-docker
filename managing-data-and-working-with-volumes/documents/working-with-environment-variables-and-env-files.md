## ARGuments & ENVironment Variables

Docker supports build-time ARGuments and runtime ENVironment variables

### ARG

- Available inside of Dockerfile, NOT accessible in CMD or any application code
- Set on image build (**docker builld**) via `--build-arg`

### ENV

- Available inside of Dockerfile & in application code
- Set via ENV in Dockerfile or via --env on **docker run**

- Example in Dockerfile

```docker
FROM node:14

WORKDIR /application

COPY package.json .

RUN npm install

COPY . .

ENV PORT 80

EXPOSE $PORT

CMD ["npm", "start"]
```

- Example in terminal (`--env PORT=8000`)

```docker
docker run -d -p 3000:8000 --rm --name feedback-app -v feedback:/application/feedback -v "/home/leonardo/Documentos/github/learning-docker/managing-data-and-working-with-volumes/projects/data-volumes-starting-setup":/application:ro -v /application/temp -v /application/node_modules --env PORT=8000 feedback-app:env
```

- Example using **.env** file

```docker
docker run -d -p 3000:8000 --rm --name feedback-app -v feedback:/application/feedback -v "/home/leonardo/Documentos/github/learning-docker/managing-data-and-working-with-volumes/projects/data-volumes-starting-setup":/application:ro -v /application/temp -v /application/node_modules --env-file ./.env feedback-app:env
```
