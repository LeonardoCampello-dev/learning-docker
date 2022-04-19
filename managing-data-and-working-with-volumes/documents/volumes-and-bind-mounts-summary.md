## Volumes - Comparison

### Anonymous Volumes (`docker run -v /application/data`)

- Created specifically for a single container
- Survives a container shutdown / restart unless `--rm` is used
- Can not be shared across containers
- Since it's anonymous, it can't be re-used (even on same image)

### Named Volumes (`docker run -v data:/application/data`)

- Created in general - not tied to any specific container
- Survives container shutdown / restart - removal via Docker CLI
- Can be shared across containers
- Can be re-used for same container (across restarts)

### Bind Mounts (`docker run -v /path/to/code:/application/code`)

- Location on host file system, not tied to any specific container
- Survives container shutdown / restart - removal on host fs
- Can be shared across containers
- Can be re-used for same container (across restarts)
