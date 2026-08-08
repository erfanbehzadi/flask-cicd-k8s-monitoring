# Flask CI/CD + Kubernetes + Monitoring

A complete DevOps project that demonstrates building, containerizing, deploying, and monitoring a simple Flask application using modern DevOps tools.

## Project Overview

This project includes:

- A simple Flask web application
- Dockerized application
- Kubernetes manifests (Deployment, Service, Ingress)
- GitLab CI/CD pipeline for building and pushing Docker images
- Basic monitoring structure with Prometheus & Grafana in mind

## Technologies Used

- Python + Flask
- Docker
- Kubernetes
- GitLab CI/CD
- Nginx Ingress
- Prometheus + Grafana

## Project Structure

```text
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
