## Containers

Read-write layer on top of image

Containers are these isolated boxes that contain our code and the environment needed to run that code.

- Isolated
- Single-task-focused
- Shareable, reproducible
- Stateless (+ volumes)

## Images

Created with instructions (layers)

The images are created with Dockerfiles or pulled from Docker Hub, these images contain the necessary code and environment as described in the Dockerfile. And so the container is just an extra thin layer on top of the image, we can run multiple containers from the same image.

- Blueprints for Containers
- Code + environment
- Read-only / does not run
- Can be built + shared
