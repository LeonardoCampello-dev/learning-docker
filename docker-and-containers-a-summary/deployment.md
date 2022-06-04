## Deployment Considerations

- Replace **Bind Mounts** with **Volumes** or **COPY**
- Multiple containers might need **multiple hosts**
- But they can also run on the **same host** (depends on application)
- **Multi-stage builds** help with apps that need a **build step**

### Control vs Ease-of-use

You can launch a **remote server**, **install Docker** and **run your containers**

- Full control but you also need to manage everything

You can use a **managed service** instead

- Less control and extra knowledge required but easier to use, less responsibility
