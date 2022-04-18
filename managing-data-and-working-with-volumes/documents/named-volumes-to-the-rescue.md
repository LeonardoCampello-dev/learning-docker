## Two types of External Data Storages

### Volumes (Managed by Docker)

- Anonymous Volumes
- Named Volumes

Docker sets up a folder / path on your host machine, exact location is unknown to you = (dev). Managed via **docker volume** commands.

A defined path in the container is mapped to the created volume / mount. e.g. `/some-path` on your hosting machine is mapped to `application/data`

Great for data which should be persistent but which you don't need to edit directly
