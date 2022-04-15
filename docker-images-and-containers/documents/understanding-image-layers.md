### [Images and layers](https://docs.docker.com/storage/storagedriver/#images-and-layers)

- A Docker image is built up from a series of layers. Each layer represents an instruction in the image’s Dockerfile. Each layer except the very last one is read-only.

- When you change a layer in an image, all subsequent layers are reconstructed.
