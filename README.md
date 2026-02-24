# MEAN Stack CRUD Application Deployment Task

## Candidate Information
* **Name:** Jaya Kiran Reddy
* **Role:** DevOps Internship Candidate
* **Deployment Date:** Feb 24, 2026

## Task Summary
Successfully containerized and deployed a full-stack MEAN application using a modern CI/CD pipeline.

### Tech Stack Used
* **Frontend:** Angular 15 (Containerized with Nginx)
* **Backend:** Node.js & Express
* **Database:** MongoDB (Official Docker Image)
* **Orchestration:** Docker Compose
* **CI/CD:** GitHub Actions
* **Cloud:** AWS EC2 (Ubuntu 22.04)
* **Reverse Proxy:** Nginx (configured inside the frontend container to route `/api` traffic)

### How to Access
* **Live URL:** http://[YOUR_AWS_PUBLIC_IP_HERE]
* **Docker Hub:** https://hub.docker.com/u/reddychinnu456959

### Pipeline Details
1.  **Build Stage:** GitHub Actions builds Docker images for both frontend and backend.
2.  **Push Stage:** Images are pushed to Docker Hub (`reddychinnu456959/mean-*`).
3.  **Deploy Stage:** The pipeline SSHes into the AWS EC2 instance, pulls the latest `docker-compose.yml`, and restarts the containers.
