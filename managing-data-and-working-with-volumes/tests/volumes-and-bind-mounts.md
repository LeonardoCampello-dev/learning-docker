### What's a "Volume" (when working with Docker)?

- A folder / file inside of a Docker container which is connected to some folder outside of the container.

### Which statement is correct?

- Volumes are managed by Docker, you don't necessarily know where the host folder (which is mapped to a container-internal path) is.

### What's true about Anonymous Volumes?

- They are removed when a container, that was started with "--rm" is stopped.

### What's the advantage of "Named Volumes"?

- They survive container removal.

### What's a "Bind Mount"?

- A path on your host machine, which you know and specified, that is mapped to some container-internal path.

### What's a typical use-case for a "Bind Mount"?

- You want to provide "live data" to the container (no rebuilding needed).

### Are Anonymous Volumes useless?

- No, you can use them to prioritize container-internal paths higher than external paths.
