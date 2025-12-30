# 🚀 Kubernetes Deployment on AWS EKS using Jenkins, Docker & Helm

## 📌 Project Overview
This project demonstrates an end-to-end **CI/CD pipeline** to deploy a containerized application on **AWS EKS (Elastic Kubernetes Service)** using **Jenkins**, **Docker**, and **Helm**.

The goal of this project is to show how a DevOps Engineer can automate:
- Application build
- Docker image creation
- Image push to Docker Hub
- Kubernetes deployment using Helm charts

---

## 🛠️ Tools & Technologies Used
- **AWS**: EC2, EKS, IAM, Load Balancer
- **Jenkins**: CI/CD automation
- **Docker**: Containerization
- **Kubernetes (EKS)**: Container orchestration
- **Helm**: Kubernetes package manager
- **Git & GitHub**: Version control
- **Linux (Amazon Linux 2023)**

---

## 🏗️ Project Architecture
1. Developer pushes code to GitHub
2. Jenkins pipeline is triggered
3. Jenkins builds Docker image
4. Docker image is pushed to Docker Hub
5. Helm deploys the application to AWS EKS
6. Application is exposed using Kubernetes LoadBalancer service

---

## 📂 Project Structure
project-2-eks/
│── app/ # Application source code
│── helm-chart/ # Helm chart for Kubernetes deployment
│ ├── templates/
│ ├── Chart.yaml
│ └── values.yaml
│── Dockerfile # Docker image configuration
│── Jenkinsfile # Jenkins CI/CD pipeline
│── .gitignore
│── README.md


---

## ⚙️ Jenkins Pipeline Stages
- **Checkout Code** from GitHub
- **Build Docker Image**
- **Push Image to Docker Hub**
- **Deploy to EKS using Helm**

---

## ☸️ Kubernetes Deployment
- Application deployed as Kubernetes **Deployment**
- Exposed using **Service (LoadBalancer)**
- Managed using **Helm charts**
- Auto-scaling and rolling updates supported

---

## 🌐 Application Access
After deployment, the application is accessible via:
- **AWS Load Balancer DNS**
- Port: `3000`

---

## 🔐 Credentials Management
- Docker Hub credentials stored securely in **Jenkins Credentials**
- Kubernetes access managed using **kubeconfig**

---

## 🚧 Current Status
- AWS account is currently suspended, so live redeployment is paused.
- Complete CI/CD pipeline setup and deployment steps are implemented and tested earlier.

---

## 🎯 Key Learnings
- Hands-on experience with AWS EKS
- Real-world Jenkins CI/CD pipeline
- Docker image lifecycle management
- Helm-based Kubernetes deployments
- Troubleshooting Jenkins agents and Docker permissions

---

## 👩‍💻 Author
**Reeta Bhagat**  
DevOps AWS Engineer (3+ years experience)

---

## 📌 Note
This project is created for **learning, practice, and interview demonstration purposes**.
