# Flask CI/CD + Kubernetes + Monitoring

A complete DevOps project that demonstrates building, containerizing, deploying, and monitoring a simple Flask application using modern tools.

## Project Overview

This project includes:

- A simple Flask web application
- Dockerized application
- Kubernetes manifests (Deployment, Service, Ingress)
- GitLab CI/CD pipeline for building and pushing Docker image
- Basic monitoring structure with Prometheus & Grafana in mind

## Technologies Used

- **Python + Flask**
- **Docker**
- **Kubernetes**
- **GitLab CI/CD**
- **Nginx Ingress**
- **Prometheus + Grafana** (structure prepared)

## Project Structure
├── app/
│   ├── app.py
│   └── requirements.txt
├── k8s/
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
├── monitoring/
├── Dockerfile
├── docker-compose.yml
├── .gitlab-ci.yml
└── README.md

## How to Run Locally

### 1. Using Docker Compose
docker-compose up --build

Then open: http://localhost:5000

###2. Build and Run Manually
docker build -t flask-cicd-app .
docker run -p 5000:5000 flask-cicd-app

Kubernetes Deployment
kubectl apply -f k8s/

GitLab CI/CD
The pipeline has two stages:

Build: Builds the Docker image and pushes it to Docker Hub
Deploy: Applies Kubernetes manifests (manual trigger)

Note: You need to set DOCKER_USER and DOCKER_PASSWORD variables in your GitLab project settings.

API Endpoints
Endpoint
/          Returns app info
/health    Health check endpoint

Author
Erfan Behzadi
GitHub: erfanbehzadi
