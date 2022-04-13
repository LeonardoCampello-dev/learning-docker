- To name a container you must use the `--name` flag

  - `docker run -p 3000:80 -d --rm --name goals-app <image_id>`
  - `docker stop goals-app`

- To name an image you must use tags:

[docker image tag](https://docs.docker.com/engine/reference/commandline/image_tag/)

> name:tag

- **name:** Defines a **group** of **possible more specialized**, images

  - Example: node

- **tag:** Defines a **specialized image within a group of images**

  - Example: 14

- **Combined:** A **unique identifier**

  - > node:14

- `docker build -t goals:latest .`
  - > goals latest 22be254ee00b 23 hours ago 949MB

`docker run -p 3000:80 -d --rm --name goals-app goals:latest `
