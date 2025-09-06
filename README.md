# Node.js + PostgreSQL App

A simple application built with **Node.js and PostgreSQL**, currently deployed on **Kubernetes (Minikube)**.  
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
```
```bash
kubectl apply -f k8s/
```
```bash
kubectl get pods -n nodejs-app
```
## Access the Node.js application in your browser
```bash
minikube service nodejs-app-service -n nodejs-app
```

## Learning Outcomes

During this project, I gained hands-on experience with:

- **Docker & Docker Compose**: Containerizing a Node.js application and running it with a PostgreSQL database locally.
- **Kubernetes (Minikube)**: Deploying apps using Deployments, Services, PersistentVolumes, and PersistentVolumeClaims.
- **Environment Variables**: Configuring the app to securely connect to the database.
- **Debugging & Networking**: Understanding how pods communicate in Kubernetes and solving connectivity issues (`EAI_AGAIN`, service discovery).
- **Comming**: Preparing the app for cloud deployment (ECS / AWS) and learning about RDS connections and credentials.


# Contact / Support

For any questions or support regarding this project, you can reach me at:

- **Email:** noureldiensami2021@gmail.com
- **LinkedIn:** [Noureldin Sami](https://www.linkedin.com/in/noureldien-sami/)
- **Website:** [Noureldin Sami](https://noureldien-sami2024.netlify.app/)  
- **GitHub Issues:** [Open an Issue](https://github.com/noureldien2021/Project-2-Serverless-Image-Processing-with-S3-and-Lambda/issues)

















