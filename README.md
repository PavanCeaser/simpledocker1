
# Static Website with Nginx and Docker

## Project Overview
This project demonstrates how to host a static website using **Nginx** and **Docker**. You will build a Docker image containing the website and run it using Nginx as a web server.

## Prerequisites
- Docker installed on your system.
- Basic understanding of Docker commands.

## Getting Started

### Step 1: Clone the Repository
```bash
git clone https://github.com/PavanCeaser/simpledocker1.git
cd simpledocker1
```

### Step 2: Build Docker Image
```bash
docker build -t my-website .
```

### Step 3: Create and Run the Docker Container
```bash
docker run -d -p 8080:80 my-website
```

### Alternative: Using Docker Compose

#### Step 1: Create Docker Compose File
Create a file named `docker-compose.yml` with the following content:
```yaml
version: '3'
services:
  web:
    build: .
    ports:
      - "8080:80"
```

#### Step 2: Build and Run the Docker Container
```bash
docker-compose up -d
```

## Accessing Your Website
Open a web browser and navigate to:
```
http://localhost:8080
```

## Common Docker Commands

### Build Docker Image
```bash
docker build -t my-website .
```

### Create and Run Docker Container
```bash
docker run -d -p 8080:80 my-website
```

### Start Docker Container
```bash
docker start <container-id>/<container-name>
```

### Stop Docker Container
```bash
docker stop <container-id>/<container-name>
```

### Remove Docker Container
```bash
docker rm <container-id>/<container-name>
```

### Remove Docker Image
```bash
docker rmi <image-id>/<image-name>
```

## Troubleshooting

### Check Docker Container Logs
```bash
docker logs <container-id>/<container-name>
```

### Verify Docker Container Status
```bash
docker ps
```

---

                    
  
