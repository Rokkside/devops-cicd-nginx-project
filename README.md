# DevOps CI/CD Pipeline with Nginx Reverse Proxy (Port 80)

## Project Overview
This project demonstrates an end-to-end CI/CD pipeline that deploys a containerized Flask application using Docker and serves it via Nginx on port 80.

## Architecture
- GitHub (Source Control)
- GitHub Actions (CI/CD)
- AWS EC2 (Compute)
- Docker (Containerization)
- Nginx (Reverse Proxy)

## Workflow
1. Developer pushes code to GitHub
2. GitHub Actions pipeline is triggered
3. Application is built as a Docker image
4. Container runs on EC2 (port 5000)
5. Nginx routes traffic from port 80 → 5000

## Technologies Used
- Python (Flask)
- Docker
- Nginx
- AWS EC2
- GitHub Actions

## Outcome
- Reverse proxy setup (port 80)
- Production-style architecture
- Foundation for Terraform automation

## Deployment Walkthrough

### 1. Project Initialization
![Project Initialization](screenshots/01-project-initialization.png)

### 2. Project Scaffolding
![Project Scaffolding](screenshots/02-project-scaffolding.png)

### 3. Application Code
![Application Code](screenshots/03-application-code.png)

### 4. Dependencies Installation
![Dependencies](screenshots/04-dependencies.png)
