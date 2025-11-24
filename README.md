# 🚀 Kubernetes MongoDB + Mongo Express Setup

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
- Mongo Express - via Port Forward / Ingress

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

# 🙌 Author

## Aayush Soni
### Cloud & Kubernetes Learner 🚀

---
