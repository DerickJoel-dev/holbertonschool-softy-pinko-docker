
# Docker Project

This project demonstrates how to build and run a web application using Docker. It includes a backend API, a frontend served by Nginx, and a proxy server that handles routing and load balancing. All components are containerized and orchestrated using Docker Compose.

---
# Tasks Overview

**Task 0 - First Docker Image**

- Create a Dockerfile based on ubuntu:latest

- Run **apt-get update** and **apt-get upgrade -y**

- Output "Hello, World!" when container runs

**Task 1 - Backend Setup**

- Use Ubuntu base image

- Install Python3, pip3, Flask

- Run a simple Flask API (/api/hello) that returns "Hello, World!"

**Task 2 - Frontend Setup**

- Use Nginx to serve a static frontend (cloned from provided repo)

- Configure Nginx to listen on port 9000

**Task 3 - Connect Frontend and Backend**

- Add dynamic content to frontend using jQuery AJAX

- Use Flask-CORS to allow cross-origin requests from frontend

**Task 4 - Docker Compose**

- Create docker-compose.yml to manage both backend and frontend services

- Expose ports so services are reachable from the host

**Task 5 - Proxy Server**

- Add a proxy service (Nginx) to route requests:

- / → frontend

- /api → backend

- Update frontend JS to send requests to /api/hello

**Task 6 - Load Balancing**

- Scale backend to 2 instances

- Use Nginx round-robin to load balance requests

- Command used: docker-compose up --scale back-end=2

---

# Technologies Used

- Docker & Docker Compose

- Python (Flask)

- HTML/CSS/JS (Frontend)

- Nginx (Static server + Proxy)

---

# Author

Derick Quinones

