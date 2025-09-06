# Node.js + PostgreSQL App

A simple application built with Node.js and PostgreSQL, currently deployed on **Kubernetes (Minikube)** for learning purposes.  
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

---
## Deploy on Minikube

1. Start Minikube:

```bash
minikube start



