Using python:3.11 as our base image with my computer and internet connection takes 121.6 seconds to build a basic Flask app. And our image size is 1.02GB.
![image](https://user-images.githubusercontent.com/77550070/276677294-a9266933-0e71-47b0-82f1-de51d44f8e06.png)
Changing the base image to python:3.11-slim decrease our build time to 19.7 seconds and size to 147MB.
![image](https://user-images.githubusercontent.com/77550070/276679736-b3028cd0-f132-43cb-9361-aa1435ac9991.png)
Smaller size and faster build time mean faster deployment, lower costs, increased security thanks to fewer components, and improved developer efficiency.  But for some Python libraries we need common Python packages that slim image doesn't contain.

For trying python:3.11-slim  <br />
```git clone https://github.com/tolgatorun/base-image-choice/ ``` <br />
then change Dockerfile's first line to  <br />
```FROM python:3.11-slim``` <br /><br />
For trying python:3-11  <br />
```git clone https://github.com/tolgatorun/base-image-choice```
