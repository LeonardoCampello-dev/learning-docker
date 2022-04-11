### What are "Images" (when working with Docker)?

- [x] Images are "blueprints" for containers which then are running instances with read and write access.

### Why do we have "Images" and "Containers"? Why not just "Containers"?

- [x] This concept allows multiple containers to be based on the same image without interfering with each other.

### What does "Isolation" mean in the context of containers?

- [x] Containers are separated from each other and have no shared data or state by default.

### What's a "Container"?

- [x] An isolated unit of software which is based on an image. A running instance of that image.

### What are "Layers" in the context of images?

- [x] Every instruction in an image creates a cacheable layer - layers help with image re-building and sharing.

### What does this command do?

```dockerfile
docker build
```

- [x] It builds an image.

### What does this command do?

```dockerfile
docker run node
```

- [x] It creates and runs a container based on the "node" image.
