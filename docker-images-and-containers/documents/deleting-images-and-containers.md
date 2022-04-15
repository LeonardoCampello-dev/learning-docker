- Command to delete a container: (only stopped containers can be deleted)

  - `docker rm <container_name || container_id>`

- Command to list images:
  - `docker images`
- Command to delete an image: (only for images that are not being used by containers)

  - `docker rmi <image_id>`

- Commando to remove all unused images:
  - [`docker image prune`](https://docs.docker.com/engine/reference/commandline/image_prune/)
  - `docker image prune -a` (Remove all unused images, not just dangling ones)
