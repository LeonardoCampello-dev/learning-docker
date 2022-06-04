## Docker containers and data

Containers are **isolated** and **stateless**

- Isolated: Containers have their own data and filesystem, detached from the host machine filesystem

  - Use **Bind Mounts** to connect host machine folders
  - `-v /local/path:/container/path`

- Stateless: They can store data internally, but data will be lost if the container is removed and replaced by a new one
  - Use **Volumes** to persist data
  - `-v NAME:/container/path`

## Docker containers and networks

Containers are isolated but **can be connected** to send requests to each other (e.g. HTTP)

- Option 1: Determine container IP and use that
  - IP might change, determining it is unecessary (manual) work
- Option 2: Create a Docker network and add both containers
  - Containers can use each other's names as request addresses
