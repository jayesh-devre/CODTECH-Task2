# CODTECH-Task3
## Containerize a web application using Docker

This project demonstrates how to containerize the 2048 game using Docker with Nginx as the web server.

### Steps to Build and Run Locally
Create the Dockerfile 

Build the Docker image:
```bash
docker build -t 2048-nginx:1.0 .
```
Run the container:
```
docker run -d -p 8080:80 --name 2048-container 2048-nginx:1.0
```
Access the 2048 game in your browser: http://localhost:8080

#### Stopping the Container

Stop the container:

```
docker stop 2048-container
```
Remove the container:
```
docker rm 2048-container
```

