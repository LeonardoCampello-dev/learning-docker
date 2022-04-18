## Understanding Data Categories / Different Kinds

### Application (Code + Environment)

- Written & provided by you (= the developer)
- Added to image and container in build phase
- "Fixed": Can't be changed once image is built
- _Read-only, hence stored in **Images**_

### Temporary App Data (e.g. entered user input)

- Fetched / Produced in running container
- Stored in memory or temporary files
- Dynamic and changing but cleared regularly
- _Read + write temporary, hence stored in **Containers**_

### Permanent App Data (e.g. user accounts)

- Fetched / Produced in running container
- Stored in files or a database
- Must not be lost if container stops / restarts
- _Read + write, permanent, stored with **Containers & Volumes**_
