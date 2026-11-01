# DevOps Website

A static website built with HTML and deployed using Docker and Nginx.

## Project Overview

This project demonstrates website containerization, web server configuration, deployment, monitoring, and troubleshooting using Docker and Nginx.

## Technologies Used

- HTML5
- Docker
- Nginx
- Git and GitHub
- PowerShell

## Project Features

- Static website served through Nginx.
- Custom Docker image built using a Dockerfile.
- Port mapping for browser access.
- Bind mounts for local development.
- Docker health checks.
- Container logs and troubleshooting.
- Container recovery and restart policy configuration.

## Build the Docker Image

```powershell
docker build -t devops-website:1.0 .
```

## Run the Container

```powershell
docker run -d --name devops-website-demo -p 8081:80 devops-website:1.0
```

Access the website at:

http://localhost:8081

## Troubleshooting Commands

View running containers:

```powershell
docker ps
```

View container logs:

```powershell
docker logs devops-website-demo
```

Inspect container configuration:

```powershell
docker inspect devops-website-demo
```

## What This Project Demonstrates

Practical experience with containerization, web server configuration, port mapping, application monitoring, troubleshooting, and container recovery.

## Future Improvement

Publish the static website through GitHub Pages to make it publicly accessible online.