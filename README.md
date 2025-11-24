# 🚀 Kubernetes MongoDB + Mongo Express Setup
<img width="1333" height="762" alt="Screenshot 2025-11-24 202013" src="https://github.com/user-attachments/assets/bf5abd37-bed8-489e-b6bf-26c9db954f5b" />


This project is a beginner-friendly Kubernetes setup where I deployed:

- MongoDB database
- Mongo Express UI
- Kubernetes Dashboard
- Exposed services using ClusterIP + Ingress + Port Forwarding

This project helped me understand how real-world Kubernetes networking works.

---

## 🧩 Tech Stack

- Kubernetes (Minikube)
- Docker
- MongoDB
- Mongo Express
- Kubernetes Dashboard
- ConfigMaps & Secrets
- Ingress Controller

---

## 🛠 What I Learned

✅ How Deployments work  
✅ Services (ClusterIP) and DNS inside K8s  
✅ How Pods communicate using Service names  
✅ Secrets & ConfigMaps  
✅ How Ingress really works  
✅ Debugging real Kubernetes networking issues  

---

## 📦 Project Architecture

User → Ingress → Service → Pod (Mongo Express)
↓
Service → Pod (MongoDB)


---

## ⚙️ How to Run This Project

### 1. Start Minikube
- minikube start

### 2.Enable Ingress
- minikube addons enable ingress

### 3. Apply Kubernetes Manifests
- kubectl apply -f mongo.yaml
- kubectl apply -f mongo-express.yaml
- kubectl apply -f dashboard-ingress.yaml

### 4. Port forward the Dashboard
- kubectl port-forward svc/kubernetes-dashboard -n kubernetes-dashboard 8443:443

### 5. Access the Services
- Kubernetes Dashboard - https://localhost:8443
<img width="1603" height="771" alt="Screenshot 2025-11-24 101302" src="https://github.com/user-attachments/assets/c6e1a012-8d4e-4451-94c2-1bee5175b774" />


<img width="1259" height="892" alt="Screenshot 2025-11-24 101248" src="https://github.com/user-attachments/assets/f659b146-e026-44aa-a742-bc6cfed010be" />


- Mongo Express - via Port Forward / Ingress

<img width="1242" height="543" alt="Screenshot 2025-11-23 153857" src="https://github.com/user-attachments/assets/ccc612ae-83a0-4396-b0d6-5c075f1bb268" />


# 📚 Key Kubernetes Concepts Used

- Pods

- Deployments

- Services

- Namespaces

- Secrets

- ConfigMaps

- Ingress

---
# 🎯 Goal

- This project was created as a stepping stone to master Kubernetes before moving to real production clusters like AWS EKS.
---

# 🙌 Author
 Aayush Soni

---
