# Springboot-Application

# DevOps Mega Project – Bank Application (AWS EKS)

## Architecture
- GitHub → Jenkins → Docker → EKS → ArgoCD → Monitoring

## Tech Stack
- Jenkins, Docker, Kubernetes (EKS), ArgoCD
- Terraform (Infrastructure)
- SonarQube, Trivy, OWASP (Security)
- Prometheus, Grafana (Monitoring)

## CI/CD Flow
1. Code pushed to GitHub
2. Jenkins pipeline triggered
3. Build Docker image
4. Scan using Trivy
5. Push to registry
6. Deploy via ArgoCD to EKS

## Screenshots
(Add Jenkins, Grafana, ArgoCD UI screenshots)

## How to Run
(terraform + kubectl steps)

## 🔗 Project Documentation
For a complete step-by-step explanation of the architecture, setup, and implementation, refer to the blog:  
👉 https://nikithajain.hashnode.dev/devops-mega-project

