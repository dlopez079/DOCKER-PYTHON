# Docker-Python

I created this project to become further understand how to create a docker image using docker compose yml file and Dockerfile.  

## Getting Started

I started the project with the app.py file which is the content of the project which will display on the webpage.  Usine the Dockerfile and the docker-compose.yml file, I created the image necessary for the project.  The requirement.txt will list the packages needed for the project.   The packages are installed on the image, not the local environment.

### DockerFile
1. The Dockerfile will fetch the python:3.7-alphine image.
2. Create the working directory in the image.
3. Utilize the Flask application.
4. Establish the host via Flask.
5. Run apk addition.
6. Copy the requirement.txt from local to image.
7. Run PIP install of the requirement list onto image.
8. Copy existing directory to image.
9. Run the application.

### docker-compose.yml
1. Run Docker Version 3.9
2. Run the 1st of 2 services: Web Service
3. Build using the current directory.
4. Use the listed ports.
5. attached volumns for the data.
6. Identify the environment
7. Run the 2nd of 2 services: redis:alphine

