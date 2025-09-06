# Node.js + PostgreSQL App

A simple application built with **Node.js and PostgreSQL**, currently deployed on **Kubernetes (Minikube)** for learning purposes.  
This project demonstrates how to containerize an app, connect it to a PostgreSQL database, and run it on Kubernetes.

---

## Features

- PostgreSQL database for data storage
- Dockerized Node.js application
- Kubernetes deployment manifests (Deployment, Service, PVC, PV)
- Minikube-compatible setup
- Optional Docker Compose for local development

---

## Project Structure

---

## Requirements

- Node.js >= 14  
- Docker / Docker Desktop  
- Minikube  
- Kubernetes CLI (`kubectl`)  
- PostgreSQL (optional for local development)

---

## Run Locally with Docker Compose

```bash
# Build and start containers
docker-compose up --build
```

## Deploy on Minikube

1. Start Minikube:

```bash
minikube start

kubectl apply -f k8s/

kubectl get pods -n nodejs-app
```
## Access the Node.js application in your browser
```bash
minikube service nodejs-app-service -n nodejs-app
```

## What I Learned

During this project, I gained hands-on experience with:

- **Docker & Docker Compose**: Containerizing a Node.js application and running it with a PostgreSQL database locally.
- **Kubernetes (Minikube)**: Deploying apps using Deployments, Services, PersistentVolumes, and PersistentVolumeClaims.
- **Environment Variables**: Configuring the app to securely connect to the database.
- **Node.js & PostgreSQL**: Implementing CRUD operations and connecting a backend server to a relational database.
- **Debugging & Networking**: Understanding how pods communicate in Kubernetes and solving connectivity issues (`EAI_AGAIN`, service discovery).
- **Git & GitHub**: Structuring a project repository, writing a professional README, and version controlling the project.
- **Optional**: Preparing the app for cloud deployment (ECS / AWS) and learning about RDS connections and credentials.




















