# 🚀 StreamOps
### End-to-End DevOps | CI/CD Automation | Docker | Kubernetes

<p align="center">
  **Automating Application Delivery with Modern DevOps Tools**
</p>

---

## 🌟 About The Project

**StreamOps** is an end-to-end DevOps project designed to automate the application delivery lifecycle using industry-standard DevOps tools and practices.

The project implements a CI/CD pipeline using **Jenkins**, integrates **SonarQube** for code quality analysis, **Trivy** for security scanning, **Docker** for containerization, and **Kubernetes** for application deployment.

The application is deployed to a Kubernetes cluster running on Minikube through a dedicated Jenkins Windows Agent.

## 🏗️ Project Architecture

```text
                  👨‍💻 Developer
                       |
                       v
                  GitHub Repo
                       |
                       v
                Jenkins Controller
                   (AWS EC2)
                       |
              +--------+--------+
              |                 |
              v                 v
         Code Checkout     Pipeline Trigger
              |
              v
         SonarQube
       Code Analysis
              |
              v
         Trivy Scan
      Filesystem Security
              |
              v
         Docker Build
              |
              v
         Trivy Scan
       Image Security
              |
              v
          Docker Hub
              |
              v
       Jenkins Windows Agent
              |
              v
          Kubernetes
           (Minikube)
              |
              v
       YouTube Clone App
```

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Cloud | AWS EC2 |
| CI/CD | Jenkins |
| Version Control | Git, GitHub |
| Code Quality | SonarQube |
| Security Scanning | Trivy |
| Containerization | Docker |
| Container Registry | Docker Hub |
| Orchestration | Kubernetes, Minikube |
| Build Tools | Maven, Node.js |
| Operating System | Linux, Windows |

## ⚡ CI/CD Pipeline

The Jenkins pipeline automates the following stages:

| Stage | Description |
|---|---|
| 📥 Checkout | Retrieves application source code from GitHub |
| 🧹 Clean Workspace | Removes previous workspace files |
| 🔍 Code Analysis | Performs static code analysis using SonarQube |
| 📦 Dependency Installation | Installs application dependencies |
| 🛡️ Filesystem Scan | Scans project files using Trivy |
| 🐳 Docker Build | Builds the application Docker image |
| 🔐 Image Scan | Scans the Docker image for vulnerabilities |
| ☁️ Image Push | Pushes the image to Docker Hub |
| ☸️ Deployment | Deploys the application to Minikube |

## 🐳 Docker Hub

The application Docker image is published to Docker Hub.

**Image Repository:** `pinshu/youtube-clone`

**Image Tag:** `latest`

## ☸️ Kubernetes Deployment

The application runs inside a Minikube Kubernetes cluster.

Kubernetes resources used:

- **Deployment:** Manages application replicas.
- **Pods:** Run application containers.
- **ReplicaSet:** Maintains the desired number of replicas.
- **Service:** Exposes the application to external access.

**Deployment Details:**
- Application: YouTube Clone
- Replicas: 2
- Container Port: 3000
- Service Type: LoadBalancer
- Target Port: 3000

## 📸 Project Highlights

- End-to-end Jenkins CI/CD pipeline.
- Jenkins controller hosted on AWS EC2.
- Integration with SonarQube.
- Filesystem and Docker image security scanning using Trivy.
- Docker image publishing to Docker Hub.
- Kubernetes deployment through a Jenkins Windows Agent.
- Application availability through Kubernetes Service.

## 🎯 Key Learnings

Working on StreamOps helped me gain hands-on experience with:

- Building Jenkins declarative pipelines.
- Configuring Jenkins tools and credentials.
- Integrating SonarQube with Jenkins.
- Building and managing Docker images.
- Performing vulnerability scans using Trivy.
- Working with Kubernetes Deployments, Pods, ReplicaSets and Services.
- Managing Minikube clusters.
- Configuring Jenkins agents for distributed pipeline execution.

## 📂 Repository

🔗 **GitHub Repository:**  
https://github.com/pkp0023/StreamOps

## 👨‍💻 Author

**Prince Kumar Pandey**

B.Tech – Computer Science & Engineering

Interested in DevOps, Cloud Infrastructure, CI/CD Automation and Kubernetes.

---

<p align="center">
  ⭐ If you find this project interesting, feel free to explore the repository!
</p>

<p align="center">
  **Built with ❤️ and DevOps practices**
</p>
