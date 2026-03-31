# SysAdmin Dashboard 🟢

A lightweight system monitoring dashboard containerized with Docker. This project serves as a practice for manual Docker image building, port mapping, and container lifecycle management.

## 📋 Overview

This dashboard is a static web application served by an **Nginx** server running inside an **Alpine Linux** container. It demonstrates the ability to:
- Create a custom `Dockerfile`.
- Map host ports to container ports.
- Manage containers using the `--rm` flag for automated cleanup.

## 🚀 Deployment Instructions

1. Build the Image
sudo docker build -t sys-admin-dash .

2. Run the Container
sudo docker run -d -p 8080:80 --name sys-dash --rm sys-admin-dash

3. Access the Dashboard
Open your web browser and go to - http://localhost:8080
