# Go Web Application

A simple and lightweight web application built with **Golang** using Go's standard `net/http` package.

The project demonstrates how to build and run a Go-based web server and can be containerized and deployed using modern DevOps tools such as **Docker, Kubernetes, Helm, and AWS EKS**.

## 🚀 Features

* Built with **Golang**
* Uses Go's standard `net/http` package
* Simple and lightweight web server
* Runs on port **8080**
* Docker-ready
* Kubernetes deployment ready
* Helm-based deployment support
* Can be deployed on **AWS EKS**

## 🛠️ Tech Stack

* **Go**
* **Docker**
* **Kubernetes**
* **Helm**
* **AWS EKS**

## 📁 Project Structure

```text
go-web-app/
│
├── main.go
├── Dockerfile
├── README.md
│
├── static/
│   └── images/
│
└── helm/
    └── go-web-app/
```

## ▶️ Running Locally

Make sure Go is installed on your system.

Clone the repository:

```bash
git clone <your-repository-url>
cd <your-project-folder>
```

Run the application:

```bash
go run main.go
```

The server will start on:

```text
http://localhost:8080
```

Open the application in your browser:

```text
http://localhost:8080/courses
```

## 🐳 Running with Docker

Build the Docker image:

```bash
docker build -t go-web-app .
```

Run the container:

```bash
docker run -d -p 8080:8080 go-web-app
```

Now access the application:

```text
http://localhost:8080/courses
```

## ☸️ Kubernetes Deployment

The application can also be deployed to a Kubernetes cluster.

Apply the Kubernetes manifests:

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

Check the deployment:

```bash
kubectl get deployments
```

Check the pods:

```bash
kubectl get pods
```

Check the service:

```bash
kubectl get svc
```

## ⛵ Helm Deployment

The application can be deployed using Helm:

```bash
helm install go-web-app ./helm/go-web-app
```

Check the Helm release:

```bash
helm list
```

Check the deployed resources:

```bash
kubectl get pods
kubectl get svc
```

## ☁️ AWS EKS Deployment

This project can be deployed to an **Amazon EKS cluster**.

After configuring the AWS CLI and Kubernetes context:

```bash
aws eks update-kubeconfig --region <your-region> --name <your-cluster-name>
```

Verify the cluster:

```bash
kubectl get nodes
```

Then deploy the application using Helm:

```bash
helm install go-web-app ./helm/go-web-app
```

## 🎯 Learning Objectives

This project was created to understand the complete journey of deploying a Go application using modern DevOps technologies:

```text
Go Application
      ↓
Docker
      ↓
Kubernetes
      ↓
Helm
      ↓
AWS EKS
and 
Argo-cd
```

<img width="1835" height="937" alt="Screenshot 2026-09-21 160403" src="https://github.com/user-attachments/assets/3df7ec13-6240-4530-90f2-e7b6b8f9a466" />

