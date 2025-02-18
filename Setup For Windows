# Minikube and kubectl Lab Setup 🚀

Easily run Kubernetes on your local machine using **Minikube** and **kubectl**! Follow this guide to set up, deploy, and manage a Kubernetes cluster step by step. 🛠️

---

## 📝 Prerequisites

- **Minikube**: Runs a local Kubernetes cluster in a virtual machine (VM).
- **kubectl**: Command-line tool to interact with Kubernetes.

---

## ⚙️ Step-by-Step Setup Guide

### 1️⃣ Install Minikube and kubectl

🔧 **Install Minikube:**
- **Linux:** `curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64`
- **macOS:** `brew install minikube`
- **Windows:** `choco install minikube`

🔧 **Install kubectl:**
- **Linux/macOS:** `curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/darwin/amd64/kubectl"`
- **Windows:** Download kubectl for Windows.

---

### 2️⃣ Start Minikube
Run:
```bash
minikube start
```
This initializes a local Kubernetes cluster inside a VM.

---

### 3️⃣ Verify Cluster 🖥️
Check if Minikube is running:
```bash
kubectl get nodes
```
You should see a node with `Ready` status. ✅

---

### 4️⃣ Create a Deployment 🛠️
Deploy an **nginx** server:
```bash
kubectl create deployment nginx --image=nginx
```
This creates a deployment named `nginx` using the official nginx image.

---

### 5️⃣ Expose the Deployment 🌐
Expose the nginx deployment as a service:
```bash
kubectl expose deployment nginx --type=NodePort --port=80
```
This makes your nginx service accessible via a NodePort.

---

### 6️⃣ Get the Service URL 🔗
Access your nginx server with:
```bash
minikube service nginx --url
```
You'll get a URL like `http://192.168.99.100:30001`.

---

### 7️⃣ Check Running Pods 🐳
View the running pods:
```bash
kubectl get pods
```
Look for the `Running` status.

---

### 8️⃣ Scale the Deployment 📈
Scale up to 3 replicas:
```bash
kubectl scale deployment nginx --replicas=3
```
Verify scaling:
```bash
kubectl get pods
```

---

### 9️⃣ Delete the Deployment 🗑️
Clean up when done:
```bash
kubectl delete service nginx
kubectl delete deployment nginx
```

---

## 📋 Kubernetes Command Flow Example
```bash
# Start Minikube
minikube start

# Verify cluster
kubectl get nodes

# Create nginx deployment
kubectl create deployment nginx --image=nginx

# Expose deployment
kubectl expose deployment nginx --type=NodePort --port=80

# Get service URL
minikube service nginx --url

# Check pods
kubectl get pods

# Scale deployment
kubectl scale deployment nginx --replicas=3

# Delete service and deployment
kubectl delete service nginx
kubectl delete deployment nginx
```

---

## 🎯 Conclusion
With **Minikube** and **kubectl**, you can effortlessly create, manage, and scale Kubernetes deployments on your local machine. 🧑‍💻 Minikube is perfect for experimenting with Kubernetes before deploying to production environments. 🚀

