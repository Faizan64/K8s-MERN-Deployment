# 🚀 WanderLust – MERN Stack Application Deployed on Kubernetes (AWS EC2)
WanderLust is a full-stack MERN (MongoDB, React, Node.js) travel blogging application.
This repository contains Kubernetes deployment manifests for running the full application on a multi-node cluster.

The project includes:

React Frontend

Node.js Backend

MongoDB Database

Redis Cache

Full Kubernetes Deployment

Exposed via NodePort on AWS EC2

Docker Images stored on Docker Hub

# 🐳 Docker Images Used
| Image    | Repository                      
| -------- | ------------------------------- 
| Frontend | `faizann16/frontend-wanderlust` 
| Backend  | `faizann16/backend-wanderlust`  


https://github.com/Faizan64/K8s-MERN-Deployment/blob/master/Screenshot%202025-11-12%20161135.png?raw=true)

# ☸️ Kubernetes Deployment

After applying all manifests i.e kubectl get all

![image alt](https://github.com/Faizan64/K8s-MERN-Deployment/blob/master/Screenshot%202025-11-12%20160326.png?raw=true)

# ✔️ Pods Running
| Service  | Status  | Age |
| -------- | ------- | --- |
| Frontend | Running | ✓   |
| Backend  | Running | ✓   |
| MongoDB  | Running | ✓   |
| Redis    | Running | ✓   |

# ✔️ Deployments Healthy

All deployments show 1/1 READY.

# ✔️ Services Exposed

| Service          | Type      | Port  |
| ---------------- | --------- | ----- |
| frontend-service | NodePort  | 31000 |
| backend-service  | NodePort  | 31100 |
| mongo-service    | ClusterIP | 27017 |
| redis-service    | ClusterIP | 6379  |







