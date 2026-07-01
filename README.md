# DevOps-Full-implementation-of-a-Go-web-application
A full implementation of a Go web application using devops principles.

# 🚀 Deploying a Go Web Application with Kubernetes & GitOps

This project demonstrates a complete cloud-native deployment pipeline for a Go web application, from containerization to automated Kubernetes deployments using GitOps.

## 📌 Workflow

1. Build a Go web application
2. Create a Docker image
3. Deploy the application to Kubernetes
4. Automate CI/CD with GitHub Actions
5. Implement GitOps using Argo CD
6. Manage deployments with Helm
7. Expose the application using an Ingress Controller

## 🛠 Tech Stack

- Go
- Docker
- Kubernetes
- GitHub Actions
- Argo CD
- Helm
- NGINX Ingress Controller

## 📂 Project Structure

```text
.
├── app/
├── Dockerfile
├── kubernetes/
│   ├── deployment.yaml
│   └── service.yaml
├── .github/
│   └── workflows/
├── helm/
│   └── go-web-app/
├── argocd/
└── README.md
```

## 🚀 Deployment Pipeline

### 1. Docker

- Build the Go application
- Create a Docker image
- Push the image to Docker Hub

### 2. Kubernetes

Deploy the application using:

- Deployment
- Service

### 3. GitHub Actions

Automate:

- Build
- Test
- Docker image creation
- Push image to Docker Hub
- Update Kubernetes manifests or Helm values

### 4. Argo CD (GitOps)

Argo CD continuously monitors the Git repository and automatically syncs changes to the Kubernetes cluster, ensuring the cluster always matches the desired state stored in Git.

### 5. Helm

Package the Kubernetes manifests into a reusable Helm chart and deploy the application to a **staging** environment with configurable values.

### 6. Ingress Controller

Expose the application externally using the **NGINX Ingress Controller**, enabling HTTP routing and preparing the application for custom domains and TLS.

## 🎯 Learning Outcomes

- Building Go applications
- Docker containerization
- Kubernetes deployments
- CI/CD automation with GitHub Actions
- GitOps workflows with Argo CD
- Helm chart development
- Kubernetes Ingress configuration
- Cloud-native application deployment

## 📄 License

This project is licensed under the MIT License.
