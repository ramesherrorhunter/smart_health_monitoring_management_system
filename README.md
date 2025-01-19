# Code Build and Deployment on K8s

## This repository showcases an end-to-end Kubernetes deployment pipeline following best practices in Kubernetes, Docker, and CI/CD automation.

## Features

- 🔄 Rolling Updates for seamless application updates
- 🔐 Enhanced Security with securityContext configurations
- 🐳 Docker Image Optimization for better performance
- 🌐 Nginx Ingress with self-signed certificates for secure communication
- ⚙️ Resource Management with defined resource requests and limits

## Prerequisites

- Docker
- Kubernetes - minikube/kind
- kubectl
- Helm
- GitHub Actions (for CI/CD)
- cert-manager and argocd installed on Kubernetes cluster

## Getting Started

### Step 1: Fork the Repository

```
git clone https://github.com/ramesherrorhunter/smart_health_monitoring_management_system\
cd smart_health_monitoring_management_system
```

### Step 2: Run CI/CD Pipeline

- Store your DOCKER_USERNAME and DOCKER_PASSWORD as GitHub secrets.
- Make cosmetic changes and push them to the main branch to trigger the GitHub Actions pipeline.
- The pipeline will:
    [1]Run security checks using Checkov and Dockle.
    [2]Build and push Docker images.
    [3]Update the Kubernetes deployment via GitOps.

## Contributing
Feel free to fork the repo and submit pull requests. Any contributions to improve the project are welcome!

## License
This project is licensed under the MIT License.