# 📄 Basic Manifest Deployment (Minikube)

This project demonstrates how to deploy a basic **nginx Deployment** in **Kubernetes** using a single manifest YAML file. It's designed to show how to define and run a scalable deployment in a **Minikube** environment.

---

## 📌 Project Overview

* **Name**: basic-manifest-deploy-minikube
* **Stack**: Kubernetes YAML, Minikube
* **Use Case**: Intro to workload management and declarative pod scaling in Kubernetes

---

## 📁 Project Structure

```
├── ejemplo.yaml       # Kubernetes Deployment manifest to run two nginx pods
```

---

## 🚀 Getting Started

### Prerequisites

* [Minikube](https://minikube.sigs.k8s.io/docs/start/)
* [kubectl](https://kubernetes.io/docs/tasks/tools/)

### Installation Steps

```bash
# 1. Start your Minikube cluster
minikube start

# 2. Apply the deployment
kubectl apply -f ejemplo.yaml

# 3. View the deployment and pod status
kubectl get deployments
kubectl get pods

# 4. Optional: View deployment details
kubectl describe deployment nginx-deployment
```

---

## 📦 Technologies Used

* **Kubernetes** – Container orchestration
* **Minikube** – Local Kubernetes cluster for development
* **YAML** – Declarative configuration for infrastructure as code

---

## 🧪 Testing and Coverage

> Manual verification using `kubectl` to inspect replica count and pod status.

---

## 🧠 Key Challenges & Learnings

* Learned to configure a `Deployment` to manage replicas
* Understood label selectors and how they bind pods to controllers
* Practiced inspecting and scaling deployments declaratively

---

## 📷 Screenshots or Live Demo

> Example CLI output:

```bash
kubectl get deployments
NAME               READY   UP-TO-DATE   AVAILABLE   AGE
nginx-deployment   2/2     2            2           10s
```

---

## 📜 License

[MIT](https://opensource.org/licenses/MIT)

---

> Created by [David Hernández](https://github.com/davidhernandez-adm) to demonstrate core Kubernetes deployment mechanics with simplicity and clarity.
