# Assignment-2

# 🚀 Kubernetes Deployment with Minikube (Python App)

This project demonstrates deploying a **Dockerized Python application** to a **local Kubernetes cluster** using **Minikube**.  
It covers containerization, Kubernetes manifests, service exposure, verification using `kubectl`, and optional ingress-based access.

---

## 🎯 Objective

- Dockerize a simple Python application
- Deploy it to a local Kubernetes cluster using Minikube
- Expose the application using a Kubernetes Service
- Verify pods and services using kubectl
- (Bonus) Configure Ingress for domain-based access

---

## 🛠 Tech Stack

- Python 3
- Flask
- Docker
- Kubernetes
- Minikube
- kubectl

---
🚀 Minikube Setup

Start Minikube using Docker driver:

minikube start --driver=docker

Build Docker Image (Inside Minikube)

Use Minikube Docker environment:

eval $(minikube docker-env)
docker build -t python-k8s-app:v1 .

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

🌍 Access the Application
minikube service python-service




