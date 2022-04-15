## Sharing via Docker Hub or Private Registry

- Docker Hub _Free Usage Possible!_

  - Official Docker Image Registry
  - Public, private and "official" Images

- Private Registry
  - Any provider / registry you want to use
  - Only your own (or team) images

### Share:

```docker
  docker push IMAGE_NAME
```

### Use:

```docker
  docker pull IMAGE_NAME
```

_Note: If you are not using Docker Hub you need to enter the full URL along with the **push** or **pull**_

- To log in to Docker Hub locally you must use the command:
  - `docker login`
- To log out of Docker Hub locally you must use the command:
  - `docker logout`
