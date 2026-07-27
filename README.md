# Project 2: Containerization and Environment Standardization

## 📌 Overview

This project demonstrates the use of Docker to containerize a web application, ensuring consistent deployment across different environments. It also includes a multi-container setup using Docker Compose.

---

## 🚀 Features

- Build a Docker image using a Dockerfile
- Containerize a static web application
- Push the Docker image to Docker Hub
- Deploy multiple containers using Docker Compose
- Environment standardization across systems

---

## 🛠️ Technologies Used

- Docker
- Docker Hub
- Docker Compose
- Nginx
- HTML

---

## 📂 Project Structure

```
docker-project/
│── Dockerfile
│── docker-compose.yml
│── index.html
│── README.md
```

---

## ⚙️ Prerequisites

- Docker Desktop
- Docker Compose
- Docker Hub Account

---

## 🔨 Build the Docker Image

```bash
docker build -t project2 .
```

---

## ▶️ Run the Container

```bash
docker run -d -p 8080:80 --name project2-container project2
```

Open in your browser:

```
http://localhost:8080
```

---

## 🐳 Push Image to Docker Hub

Login:

```bash
docker login
```

Tag the image:

```bash
docker tag project2 <YOUR_DOCKERHUB_USERNAME>/project2:v1
```

Push the image:

```bash
docker push <YOUR_DOCKERHUB_USERNAME>/project2:v1
```

---

## 📦 Multi-Container Deployment

Start the services:

```bash
docker compose up -d
```

Check running containers:

```bash
docker compose ps
```

Stop the services:

```bash
docker compose down
```

---

## 📸 Output

- Docker image created successfully
- Container running successfully
- Application accessible at:

```
http://localhost:8080
```

- Docker image uploaded to Docker Hub
- Multi-container setup running using Docker Compose

---

## 📚 Learning Outcomes

- Understanding Docker images and containers
- Writing Dockerfiles
- Working with Docker Hub
- Managing multi-container applications
- Environment standardization using Docker

---

## 👨‍💻 Author

**Sanidhya Gupta**

B.Tech CSE (AI & Data Science)

Poornima University, Jaipur

---

## 📄 License

This project is created for educational and internship purposes.
