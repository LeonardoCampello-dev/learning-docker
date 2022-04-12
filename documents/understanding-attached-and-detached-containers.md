[Docker attached vs detached article](https://www.java4coding.com/contents/docker/docker-attached-vs-detached-mode#:~:text=In%20the%20attached%20mode%2C%20Docker,the%20background%20of%20your%20terminal.)

- `Docker run` by default starts a container in attached mode
- `Docker start` by default starts a container in detached mode

In detached mode we can't see any information from the container in the console, for example a `console.log()`

- To start a container in detached mode, you must use the `-d` flag:

  - `docker run -p 3000:80 -d <container_id>`

- To get information about the container again, there are two ways:

  - `docker attach <container_name || container_id>`
  - `docker logs <container_name || container_id>`
    - `docker logs -f <container_name || container_id>`

- To start a container in attached mode, you must use the `-a` flag:
  - `docker start -a <container_name || container_id>`
