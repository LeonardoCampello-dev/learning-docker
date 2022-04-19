## Understanding Container / Volume Interaction

- Volume (`some-path`)
- Bind Mount (`some-other-path`)

- Container

  - `/application/data`
    - _some-file.txt_
    - _file2.txt_
  - `/application/code`

- Volumes are mounted into Container
- Container data is **stored in volume**

```docker
docker run -d -p 3000:80 --rm --name feedback-app -v feedback:/application/feedback -v "/home/leonardo/Documentos/github/learning-docker/managing-data-and-working-with-volumes/projects/data-volumes-starting-setup":/application -v /application/node_modules feedback-node:volumes
```

- `-v "/home/leonardo/Documentos/github/learning-docker/managing-data-and-working-with-volumes/projects/data-volumes-starting-setup":/application`
  - Volume to share updated application data with the container
  - Problem: the data on this volume fully subscribes to the container data, so we end up losing the `node_modules` folder that exists only in the container

`-v /application/node_modules`

- Anonymous volume to solve the problem of subscribing to `node_modules`, Docker follows the rule of keeping the path more specific, this way we have the updated data of the application and still keep the `node_modules`
