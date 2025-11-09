<p align="center">
  <img src="https://github.com/momna-shahid17/ci-cd-pipeline-project/blob/main/banner.png" alt="Momna Shahid — DevOps & Cloud Engineer Banner" width="100%"/>
</p>

# 🚀 CI/CD Pipeline: Flask + Docker + GitHub Actions + Terraform + AWS

## Overview 🎯
This project demonstrates a **full-stack CI/CD pipeline** using **GitHub Actions**, **Docker**, **Terraform**, and **AWS EC2** to automate the deployment of a **Flask web application**. The pipeline handles everything from building and testing the application to deploying it on a cloud server, showcasing modern DevOps practices.

### Tech Stack:
- **Flask**: A Python-based micro web framework for building the app.
- **Docker**: For containerizing the application.
- **GitHub Actions**: For continuous integration and deployment (CI/CD).
- **AWS EC2**: Cloud infrastructure for hosting the app.
- **Terraform**: Infrastructure as code (IaC) for provisioning AWS resources.
- **Docker Hub**: For storing and managing the Docker image.

---

## 🚀 Project Flow
1. **Flask app** developed and containerized using Docker.
2. **GitHub Actions** is triggered upon code push to the `main` branch.
3. **Docker image** is built and pushed to **Docker Hub**.
4. **AWS EC2** instance is provisioned using **Terraform**.
5. **GitHub Actions** SSHs into the EC2 instance and deploys the Docker container.

---

## 🔧 Prerequisites

### Environment Setup
Make sure you have the following installed:
- **Git**: For version control
- **Docker**: For containerization
- **Terraform**: For provisioning AWS resources
- **AWS CLI**: For managing AWS resources
- **Python**: To run the Flask app

You’ll also need accounts for:
- **GitHub**: To store and manage your code repository.
- **Docker Hub**: To store the Docker image.
- **AWS**: To provision cloud resources.

### GitHub Secrets
In your GitHub repository, you need to configure the following secrets under **Settings → Secrets**:

- **DOCKERHUB_USERNAME**: Your Docker Hub username.
- **DOCKERHUB_TOKEN**: Your Docker Hub access token.
- **EC2_HOST**: Public IP address of the EC2 instance (output from Terraform).
- **EC2_USER**: `ubuntu` (for Ubuntu AMI) or `ec2-user` (for Amazon Linux).
- **EC2_SSH_PRIVATE_KEY**: The private key content from your SSH keypair for EC2.

---

## 🖥️ Running the Project Locally

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/ci-cd-pipeline-project.git
cd ci-cd-pipeline-project
