
---

# Flask App Dockerized

## Project Overview
This project contains a simple **Flask** web application, which is dockerized for easy deployment. By containerizing the application, you can run it consistently across different environments.

## Prerequisites
- **Docker** installed on your system.
- Basic understanding of **Docker** and **Flask**.

## Getting Started

### Step 1: Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### Step 2: Build the Docker Image
```bash
docker build -t flask-app-d1 .
```

### Step 3: Run the Docker Container
```bash
docker run -d -p 5000:5000 flask-app-d1
```

## Accessing Your Application
Open a web browser and go to:
```
http://localhost:5000
```

## Common Docker Commands

### Build Docker Image
```bash
docker build -t flask-app-d1 .
```

### Run Docker Container
```bash
docker run -d -p 5000:5000 flask-app-d1
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

## Project Structure
- `app.py`: Contains the Flask application code.
- `requirements.txt`: Lists the dependencies for the Flask app.
- `Dockerfile`: Defines the Docker image configuration.
- `README.md`: The file you're reading now.

---

