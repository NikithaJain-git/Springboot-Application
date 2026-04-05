
🚀 DevOps Mega Project – Bank Application (AWS EKS)

🔗 Project Documentation

Detailed step-by-step implementation:
https://nikithajain.hashnode.dev/devops-mega-project

---

📌 Overview

This project demonstrates an end-to-end DevOps and DevSecOps pipeline for deploying a microservices-based Spring Boot Bank Application on AWS EKS.

It covers the complete lifecycle from code commit to production deployment using CI/CD, containerization, GitOps, and monitoring tools.

---

🏗 Architecture

"Architectural flow"

🔁 Flow:

GitHub → Jenkins → Docker → Docker hub → AWS EKS → ArgoCD → Prometheus & Grafana

---

⚙️ Tech Stack

- CI/CD: Jenkins
- Containerization: Docker
- Container Registry: Docker hub
- Orchestration: Kubernetes (AWS EKS), Helm
- Cloud: AWS (EC2, VPC, IAM, EKS)
- GitOps: ArgoCD
- DevSecOps: SonarQube, Trivy, OWASP Dependency Check
- Monitoring: Prometheus, Grafana


---

🚀 CI/CD Pipeline Flow

1. Developer pushes code to GitHub
2. Jenkins pipeline is triggered automatically
3. Application is built and packaged
4. Docker image is created using Dockerfile
5. Image is scanned using Trivy for vulnerabilities
6. Image is pushed to Amazon ECR
7. ArgoCD detects changes and deploys to AWS EKS cluster
8. Application is monitored using Prometheus and Grafana

---

📁 Project Structure

.
├── Jenkinsfile        # CI/CD pipeline definition
├── Dockerfile         # Application containerization
├── kubernetes/        # Kubernetes manifests
├── helm/              # Helm charts
├── terraform/         # Infrastructure provisioning (if applicable)

---

🔐 DevSecOps Implementation

- Integrated SonarQube for static code analysis
- Used Trivy for container vulnerability scanning
- Implemented OWASP Dependency Check for identifying vulnerable dependencies

---

📊 Monitoring & Logging

- Configured Prometheus for metrics collection
- Built dashboards using Grafana for visualization
- (Optional) Implemented centralized logging using EFK stack

---

▶️ How to Run (High-Level Steps)

1. Provision infrastructure using Terraform
2. Build Docker image using Dockerfile
3. Push image to Docker hub
4. Deploy application using Kubernetes manifests / Helm charts
5. Configure ArgoCD for GitOps-based deployment
6. Monitor application using Prometheus and Grafana

---

📸 Screenshots

Add screenshots for better understanding:

- Jenkins Pipeline Execution
- ArgoCD Application Dashboard
- Kubernetes Pods / Services
- Grafana Monitoring Dashboard

---

💡 Key Achievements

- Reduced deployment time by 40% using CI/CD automation
- Improved deployment consistency and reliability
- Implemented secure DevSecOps pipeline
- Built scalable and self-healing Kubernetes-based architecture

---

📖 Additional Resources

- Blog: https://nikithajain.hashnode.dev/devops-mega-project
- LinkedIn Post: https://www.linkedin.com/posts/nikithajainn_devops-kubernetes-ciabrcd-activity-7314904216949428225-i4Mh

---

