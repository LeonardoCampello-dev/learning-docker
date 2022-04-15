### What's the result of these commands?

```docker
docker build -t myimage .
docker run --name mycontainer myimage
docker stop mycontainer
```

- **answer:** An image is created, a container is started and then stopped. Both, image and container, have a name assigned by the developer.

### Assume that these commands were executed:

```docker
docker build -t myimage:latest .
docker run --name mycontainer --rm myimage
docker stop mycontainer
```

- **answer:** `docker rm my container`

### What's the idea behind image tags?

- **answer:** An image can have a name and then multiple "versions" of that image attached on the same name.

### Do you have to assign custom image tags and container names?

- **answer:** No, Docker auto-assigns names and ids.
