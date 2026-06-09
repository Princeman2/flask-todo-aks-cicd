# 🚀 CI/CD Pipeline for Flask Todo App on Azure AKS

Fully automated Continuous Integration and Continuous Deployment pipeline using GitHub Actions for a Python Flask application deployed on Azure Kubernetes Service.

![GitHub Actions Workflow](github-actions-success.png)

## ✨ Project Overview

Every time code is pushed to the `main` branch, GitHub Actions automatically:
- Builds a new Docker image
- Pushes it to Docker Hub
- Deploys the updated version to Azure AKS

**Live Application:** http://20.164.127.244

## 🛠️ Tech Stack

- **Backend**: Python + Flask + PostgreSQL
- **Containerization**: Docker
- **CI/CD**: GitHub Actions
- **Orchestration**: Kubernetes (AKS)
- **Cloud**: Microsoft Azure

## 📸 Pipeline Screenshots

![GitHub Actions Success](github-actions-sucess.png)  
*Complete CI/CD workflow running successfully*

![CI/CD Detailed Logs](ci-cd-logs.png)  
*Build, Push to Docker Hub, and Deploy steps*

![Git Commit & Push](git-commit-push.png)  
*Triggering the pipeline with a code change*

![Live Updated Application](live-app-v4.png)  
*New version deployed automatically*

![Kubernetes Status After Deploy](kubectl-after-deploy.png)  
*Pods and Services after successful deployment*

![Docker Hub Image](docker-hub-image.png)  
*Latest image successfully pushed to Docker Hub*

## How the Pipeline Works

1. Developer makes changes and pushes to GitHub
2. GitHub Actions automatically triggers
3. Builds and tests Docker image
4. Pushes image to Docker Hub
5. Deploys new version to Azure AKS with zero downtime

## What I Learned

- Building end-to-end CI/CD pipelines
- Secure secret management in GitHub Actions
- Automating Docker builds and Kubernetes deployments
- Azure authentication in CI/CD workflows
- Monitoring and troubleshooting automated deployments

## How to Deploy Manually

```bash
kubectl apply -f k8s/
