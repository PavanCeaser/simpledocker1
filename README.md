
Static Website with Nginx and Docker
Project Overview
This project hosts a static website using Nginx and Docker.
Prerequisites
Docker installed on your system
Basic understanding of Docker commands
Getting Started
Step 1: Clone Repository
Bash
git clone https://github.com/PavanCeaser/simpledocker1.git                    
  
cd your-repo-name
Step 2: Build Docker Image
Bash
docker build -t my-website .
Step 3: Create Docker Container
Bash
docker run -d -p 8080:80 my-website
Alternative: Using Docker Compose
Step 1: Create Docker Compose File
Create a file named docker-compose.yml:
YAML
version: '3'
services:
  web:
    build: .
    ports:
      - "8080:80"
Step 2: Build and Run Docker Container
Bash
docker-compose up -d
Accessing Your Website
Open a web browser and navigate to:
http://localhost:8080
Docker Commands
Build Docker Image
Bash
docker build -t my-website .
Create Docker Container
Bash
docker run -d -p 8080:80 my-website
Start Docker Container
Bash
docker start container-id/container-name
Stop Docker Container
Bash
docker stop container-id/container-name
Remove Docker Container
Bash
docker rm container-id/container-name
Remove Docker Image
Bash
docker rmi image-id/image-name
Troubleshooting
Check Docker container logs:
Bash
docker logs container-id/container-name
Verify Docker container status:
Bash
docker ps
