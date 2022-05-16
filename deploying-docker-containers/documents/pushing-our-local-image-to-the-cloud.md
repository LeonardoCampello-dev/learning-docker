## Deploy Source Code vs Image

- Option 1: Deploy Source (Unnecessary complexity)
  - Build image on remote machine
  - Push source code to remote machine run docker build and then docker run
- Option 2: Deploy Built Image (Avoid unnecessary remote server work)
  - Build image before deployment (e.g. on local machine)
  - Just execute docker run
