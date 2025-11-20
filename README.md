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

<br/>


<img width="1920" height="1020" alt="Image" src="https://github.com/user-attachments/assets/f00620f8-e80c-40a9-843a-e214d006b866" />

# ☸️ Kubernetes Deployment

After applying all manifests i.e kubectl get all
<br/>

<img width="1920" height="1020" alt="Image" src="https://github.com/user-attachments/assets/d26e0d1e-294d-41c7-8422-23a3311ad6e9" />

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

# 🌐 Public Access (AWS EC2 NodePort)

## Frontend UI fully accessible 
<br/>

<img width="1920" height="1020" alt="Image" src="https://github.com/user-attachments/assets/340b8dcc-7256-4ebf-bdae-250544021e85" /> <br/>
<br/>
<img width="1920" height="1020" alt="Image" src="https://github.com/user-attachments/assets/aaf24913-7f33-410c-b72e-84ef8e47fb81" />

## Backend live
<br/>

<img width="1920" height="1020" alt="Image" src="https://github.com/user-attachments/assets/31b5cd29-9420-4874-93df-73a006f845b6" />
<br/>

Both services were successfully tested and working on the deployed cluster.

# AWS EC2 master & worker nodes
<br/>

<img width="1920" height="1020" alt="Image" src="https://github.com/user-attachments/assets/c9af0594-cecb-4518-a872-ccbd00ef6d58" />









