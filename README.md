# Automated Microservices Deployment with Helm & Helmfile 🚀

This repository provides a **streamlined way to deploy and manage microservices on Kubernetes** using Helm, Helmfile, and simple Bash scripts. It simplifies the entire deployment lifecycle, from installation to cleanup, making microservices management effortless.

---

## 🛠️ Tech Stack

- Kubernetes  
- Helm  
- Helmfile  
- Bash  

> Tested on **Minikube** and **Linode Kubernetes Engine**.

---

## ⚙️ Prerequisites

Ensure the following tools are installed on your system (macOS instructions shown):

```bash
# Install Helm
brew install helm

# Install Helmfile
brew install helmfile

# Install Minikube
brew install minikube

# Start Kubernetes cluster
minikube start
```
## 🚀 Getting Started
You can deploy microservices using Bash scripts for a quick start or Helmfile for more control.

# Option 1: Deploy with Bash Scripts

Quick and easy deployment:
```bash
# Install all microservices
./install.sh

# Uninstall all microservices
./uninstall.sh
```

# Option 2: Deploy with Helmfile

Directly manage Helm charts:

```bash
# Deploy and synchronize all Helm charts
helmfile sync
 
# Destroy and remove all deployed charts
helmfile destroy
```

## ✅ Verifying the Deployment

After deployment, check your Kubernetes cluster to ensure microservices are running correctly:

```bash
# View running pods
kubectl get pods

# View exposed services
kubectl get services

# View deployed applications
kubectl get deployments
```
