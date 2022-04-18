## Understanding Volumes

Volumes are **folders on your host machine** hard drive which are **mounted** ("made available", mapped) **into containers**

Host (Your Computer)

- `some-path/` <==> `/app/user-data`

- Volumes **persist if a container shuts down.** If a container (re-)starts and a mounts a volume, any data inside of that volume is **available in the container.**
- A container **can write** data into a volume **and read** data from it.
