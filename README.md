# DevOps CI/CD Pipeline with Nginx Reverse Proxy (Port 80)

## Project Overview

This project demonstrates an end-to-end CI/CD pipeline that deploys a containerized Flask application using Docker and serves it via Nginx on port 80.

## Architecture Overview

This project demonstrates a complete CI/CD pipeline using:

- GitHub Actions for automation
- Docker for containerization
- AWS EC2 for compute
- Nginx as a reverse proxy (port 80 → 5000)

---

## Workflow

1. Developer pushes code to GitHub  
2. GitHub Actions pipeline is triggered  
3. Docker image is built  
4. Container runs on EC2 (port 5000)  
5. Nginx routes traffic from port 80 → 5000  

---

## Technologies Used

- Python (Flask)
- Docker
- Nginx
- AWS EC2
- GitHub Actions

---

## Deployment Walkthrough

### 1. Project Initialization
![Step 1](screenshots/01-project-initialization.png)

### 2. Project Scaffolding
![Step 2](screenshots/02-project-scaffolding.png)

### 3. Application Code
![Step 3](screenshots/03-application-code.png)

### 4. Dependencies Installation
![Step 4](screenshots/04-dependencies.png)

---

## Docker & Containerization

### 5. Flask App Running (Port 5000)
![Step 5](screenshots/05-flask-public-ip.png)

### 6. Flask Logs Verification
![Step 6](screenshots/06-flask-logs.png)

### 7. Dockerfile Setup
![Step 7](screenshots/07-dockerfile.png)

### 8. Docker Image Build
![Step 8](screenshots/08-docker-build.png)

### 9. Container Running (Pre-Nginx)
![Step 9](screenshots/09-container-pre-nginx.png)

---

## Nginx Reverse Proxy Setup

### 10. Nginx Started (Port Conflict Resolved)
![Step 10](screenshots/10-nginx-started.png)

### 11. Nginx Running on Port 80
![Step 11](screenshots/11-nginx-running.png)

### 12. Flask Backend Behind Nginx (Port 5000)
![Step 12](screenshots/12-flask-backend.png)

### 13. Nginx Reverse Proxy Configuration
![Step 13](screenshots/13-nginx-config.png)

### 14. Application Served via Nginx (Port 80)
![Step 14](screenshots/14-nginx-served.png)

### 15. Port Validation (80 → 5000)
![Step 15](screenshots/15-port-validation.png)

---

## CI/CD Pipeline (GitHub Actions)

### 16. GitHub Repository Setup
![Step 16](screenshots/16-github-repo.png)

### 17. Repository Cleanup (.gitignore)
![Step 17](screenshots/17-repo-cleanup.png)

### 18. Project Documentation
![Step 18](screenshots/18-project-docs.png)

### 19. GitHub Actions Workflow
![Step 19](screenshots/19-github-actions-workflow.png)

### 20. Pipeline Execution Success
![Step 20](screenshots/20-github-actions-run.png)

---

## Outcome

- Production-style reverse proxy architecture  
- Automated CI/CD deployment pipeline  
- Publicly accessible application via port 80  
- Clean DevOps workflow from code → deployment  

---

## Next Steps

- Terraform infrastructure automation  
- HTTPS (SSL via Nginx + Certbot)  
- Load balancing & scaling  
