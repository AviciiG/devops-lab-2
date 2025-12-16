# DevOps Final Project - Rasul

This project is a ToDo application developed with Python (Flask) and PostgreSQL, demonstrating a full DevOps lifecycle.

## Architecture [cite: 111]
- **App:** Python Flask (Port 5000/8080)
- **Database:** PostgreSQL 13 (Port 5432)
- **Containerization:** Docker & Docker Compose
- **Orchestration:** Kubernetes (Minikube/Kind manifests)
- **CI/CD:** Jenkins Pipeline
- **IaC:** Ansible Playbook

## Setup Instructions [cite: 112]

### 1. Run with Docker Compose
```bash
docker-compose up --build
```
Access the app at: http://localhost:8080

### 2. Jenkins
Jenkins is running in a container on port 8081.
pipeline script is located in `Jenkinsfile_Rasul`.

### 3. Kubernetes
Apply manifests from the `k8s/` directory:
```bash
kubectl apply -f k8s/
```

## Project Files [cite: 118]
- Dockerfile -> `app/Dockerfile_Rasul`
- Jenkinsfile -> `Jenkinsfile_Rasul`
- Playbook -> `ansible/playbook_Rasul.yml`
- K8s Manifests -> `k8s/*_Rasul.yaml`
