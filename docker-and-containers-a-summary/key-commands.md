## Key commands

Build an image based on **Dockerfile**

`docker build -t NAME:TAG .`

- NAME = Image name
- TAG = Image version or category
- . = Build context (where is the Dockerfile and where the image will be built)

Run a container based on a **remote or local image**

`docker run --name NAME --rm -d IMAGE`

- `--name NAME` = Container name
- `--rm` = Remove once stopped
- `-d` = Start container in detached mode

Share (push) an Image to a **Registry** (default: **DockerHub**)

`docker push REPOSITORY/NAME:TAG`

Fetch (pull) an Image from a **Registry** (default: **DockerHub**)

`docker pull REPOSITORY/NAME:TAG`
