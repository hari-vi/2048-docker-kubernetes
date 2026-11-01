# 2048 Game – Docker & Kubernetes Deployment

## Project Overview

This project demonstrates containerization and deployment of an existing open-source 2048 web application using Docker and Kubernetes.

The application is packaged using Docker with NGINX Alpine and deployed on a local Kubernetes cluster using Kind.

## Technologies Used

- Docker
- Kubernetes
- Kind
- NGINX
- HTML
- CSS
- JavaScript
- Git and GitHub

## My Contributions

- Created a Dockerfile using the lightweight NGINX Alpine image.
- Containerized the existing 2048 web application.
- Built and tested Docker images locally.
- Deployed the application using Kubernetes.
- Configured Kubernetes Deployment and NodePort Service.
- Accessed the application through Google Chrome.

## Architecture

Browser → NodePort Service → Kubernetes Pod → Docker Container → NGINX

## How to Run

### 1. Build Docker Image

```bash
docker build -t 2048_game:latest .
```

### 2. Deploy to Kubernetes

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

### 3. Verify Deployment

```bash
kubectl get pods
kubectl get services
```

### 4. Access Application

http://localhost:30958

## Credits and License

The original 2048 game was created by Gabriele Cirulli.

Original repository:
https://github.com/gabrielecirulli/2048

The original application is distributed under the MIT License.

This repository uses the original open-source game to demonstrate Docker containerization and Kubernetes deployment.

The original copyright and license notices are retained.

My contributions include Docker configuration, containerization, Kubernetes deployment, and service exposure.