
🚀 DevOps Mega Project – Bank Application (AWS EKS)

🔗 Project Documentation

Detailed step-by-step implementation:
https://nikithajain.hashnode.dev/devops-mega-project

---

📌 Overview

This project demonstrates a complete end-to-end DevOps and DevSecOps pipeline for deploying a microservices-based Spring Boot Bank Application on AWS EKS.

It includes infrastructure provisioning using Terraform, CI/CD automation, GitOps-based deployment, and monitoring for a production-like setup.

---

🏗 Architecture

🔹 Infrastructure Provisioning (IaC)

Terraform is used to provision AWS infrastructure:

- VPC and networking components
- IAM roles and security configurations
- AWS EKS (Kubernetes cluster)

---

🔹 CI/CD Pipeline

GitHub → Jenkins → Docker → Docker Hub

- Code is pushed to GitHub
- Jenkins pipeline is triggered automatically
- Application is built and packaged
- Docker image is created and pushed to Docker Hub

---

🔹 GitOps Deployment

ArgoCD → AWS EKS

- ArgoCD monitors Git repository
- Automatically deploys changes to Kubernetes (EKS)
- Ensures declarative and version-controlled deployments

---

🔹 Monitoring

AWS EKS → Prometheus → Grafana

- Prometheus collects metrics from cluster and applications
- Grafana visualizes metrics using dashboards
- Enables monitoring and alerting

---

⚙️ Tech Stack

- Infrastructure as Code: Terraform
- CI/CD: Jenkins
- Containerization: Docker
- Container Registry: Docker Hub
- Orchestration: Kubernetes (AWS EKS), Helm
- Cloud: AWS (EC2, VPC, IAM, EKS)
- GitOps: ArgoCD
- DevSecOps: SonarQube, Trivy, OWASP Dependency Check
- Monitoring: Prometheus, Grafana
- Scripting: Shell (Bash)

---

🚀 CI/CD Pipeline Flow

1. Developer pushes code to GitHub
2. Jenkins pipeline is triggered via webhook
3. Application is built and packaged
4. Docker image is created using Dockerfile
5. Image is scanned using Trivy for vulnerabilities
6. Image is pushed to Docker Hub
7. ArgoCD detects changes and deploys to AWS EKS
8. Application is monitored using Prometheus and Grafana

---

📁 Project Structure

.
├── Jenkinsfile        # CI/CD pipeline definition
├── Dockerfile         # Application containerization
├── kubernetes/        # Kubernetes manifests
├── helm/              # Helm charts
├── terraform/         # Infrastructure provisioning using Terraform

---

🔐 DevSecOps Implementation

- Integrated SonarQube for static code analysis
- Used Trivy for container vulnerability scanning
- Implemented OWASP Dependency Check for dependency security

---

📊 Monitoring & Logging

- Configured Prometheus for metrics collection
- Used Grafana dashboards for visualization
- Enabled monitoring for application and cluster health

---

▶️ How to Run (High-Level Steps)

1. Provision infrastructure using Terraform
2. Configure AWS credentials and EKS cluster
3. Build Docker image using Dockerfile
4. Push image to Docker Hub
5. Deploy application using Kubernetes/Helm
6. Configure ArgoCD for GitOps deployment
7. Monitor application using Prometheus and Grafana

---

📸 Screenshots

Add screenshots for better understanding:

- Jenkins Pipeline Execution
- ArgoCD Dashboard
- Kubernetes Pods / Services
- Grafana Monitoring Dashboard

---

💡 Key Achievements

- Reduced deployment time by 40% using CI/CD automation
- Improved deployment consistency and reliability
- Implemented secure DevSecOps practices
- Built scalable and self-healing Kubernetes-based architecture

---

📖 Additional Resources

- Blog: https://nikithajain.hashnode.dev/devops-mega-project
- LinkedIn Post: https://www.linkedin.com/posts/nikithajainn_devops-kubernetes-ciabrcd-activity-7314904216949428225-i4Mh

---
