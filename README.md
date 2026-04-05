🚀 DevOps Mega Project – Bank Application (AWS EKS)

🔗 Project Documentation

Detailed step-by-step implementation:
https://nikithajain.hashnode.dev/devops-mega-project

---

📌 Overview

This project demonstrates a complete end-to-end DevOps and DevSecOps pipeline for deploying a microservices-based Spring Boot Bank Application on AWS EKS.

It includes infrastructure provisioning using Terraform, CI/CD automation, GitOps-based deployment using ArgoCD, and monitoring for a production-like setup.

---

🏗 Architecture

"Architecture Diagram" (./architecture.png)

The architecture represents a layered DevOps workflow:

🔹 Infrastructure Provisioning (IaC)

Terraform is used to provision AWS infrastructure including:

- VPC and networking components
- IAM roles and security configurations
- AWS EKS (Kubernetes cluster)

---

🔹 CI/CD Pipeline

GitHub → Jenkins → Docker → Docker Hub

- Developers push code to GitHub
- Jenkins pipeline is triggered automatically
- Application is built and packaged
- Docker image is created using Dockerfile
- Image is pushed to Docker Hub

---

🔹 GitOps Deployment

ArgoCD → AWS EKS

- ArgoCD continuously monitors the Git repository
- Automatically syncs changes to Kubernetes (EKS)
- Eliminates manual deployments and ensures consistency

---

🔹 Monitoring

AWS EKS → Prometheus → Grafana

- Prometheus collects application and cluster metrics
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

🚀 CI/CD & GitOps Flow

1. Developer pushes code to GitHub
2. Jenkins pipeline is triggered automatically
3. Application is built and packaged
4. Docker image is created using Dockerfile
5. Image is scanned using Trivy for vulnerabilities
6. Image is pushed to Docker Hub
7. ArgoCD detects changes in Git repository
8. ArgoCD automatically syncs and deploys application to AWS EKS
9. Application is monitored using Prometheus and Grafana

---

📁 Project Structure

.
├── Jenkinsfile        # CI/CD pipeline definition
├── Dockerfile         # Application containerization
├── kubernetes/        # Kubernetes manifests
├── helm/              # Helm charts

├── terraform/         # Infrastructure provisioning using Terraform

---

▶️ How Deployment Works

# Step 1: Provision infrastructure using Terraform
terraform init

terraform apply

# Step 2: Configure kubectl for EKS
aws eks --region <region> update-kubeconfig --name <cluster-name>

# Step 3: Push code to GitHub
# Jenkins builds and pushes Docker image to Docker Hub

# Step 4: ArgoCD automatically syncs and deploys application

Application deployment is handled using ArgoCD (GitOps approach).
Any changes pushed to the Git repository are automatically detected and deployed to the EKS cluster.

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

📸 Screenshots

Add screenshots for better understanding:

- Jenkins Pipeline Execution
- ArgoCD Dashboard
- Kubernetes Pods / Services
- Grafana Monitoring Dashboard

---

⚡ Challenges & Learnings

- Implementing CI/CD pipeline automation using Jenkins
- Understanding Kubernetes deployments and service exposure
- Setting up GitOps workflow using ArgoCD
- Integrating security scanning into CI/CD pipeline
- Monitoring application performance using Prometheus and Grafana

---

💡 Key Achievements

- Reduced deployment time by 40% using CI/CD automation
- Improved deployment consistency and reliability
- Eliminated manual deployments using GitOps approach
- Built scalable and self-healing Kubernetes-based architecture

---

📖 Additional Resources

- Blog: https://nikithajain.hashnode.dev/devops-mega-project
- LinkedIn Post: https://www.linkedin.com/posts/nikithajainn_devops-kubernetes-ciabrcd-activity-7314904216949428225-i4Mh

---
