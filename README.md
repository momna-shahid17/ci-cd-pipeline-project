# 🚀 CI/CD Pipeline: Flask + Docker + GitHub Actions + Terraform + AWS

## Overview 🎯
This project demonstrates a complete **CI/CD pipeline** using **GitHub Actions**, **Docker**, **Terraform**, and **AWS EC2** to automate the deployment of a **Flask web application**. It is an end-to-end DevOps pipeline that includes:

1. **Flask app** running in a Docker container
2. **GitHub Actions** for CI/CD automation
3. **Terraform** to provision **AWS EC2** instances
4. **Docker Hub** to store and manage container images

This project is a **real-world application** of DevOps best practices, showcasing how to automate build, testing, deployment, and cloud infrastructure provisioning.

## 💡 Tech Stack
- **Flask** - A Python-based micro web framework
- **Docker** - For containerization of the Flask app
- **GitHub Actions** - Continuous integration and deployment (CI/CD)
- **AWS EC2** - Cloud infrastructure for hosting the app
- **Terraform** - Infrastructure as Code (IaC) for managing AWS resources
- **Docker Hub** - Container registry for storing images

## 🚀 Project Flow
1. **Flask app** is developed and containerized using Docker.
2. **GitHub Actions** builds and tests the Docker image automatically whenever new code is pushed to the `main` branch.
3. The **Docker image** is pushed to **Docker Hub**.
4. **Terraform** provisions an **AWS EC2** instance and installs Docker.
5. The **GitHub Actions** workflow SSHs into the EC2 instance and deploys the app by pulling the latest image from Docker Hub.

---

## 🔧 Prerequisites

### 🚀 Environment Setup
Before you begin, ensure the following tools are installed:
- **Git** for version control
- **Docker** for containerization
- **Terraform** for provisioning AWS resources
- **AWS CLI** for managing AWS resources
- **Python** for the Flask app

You will also need:
- A **GitHub account** (to store your code and run GitHub Actions)
- A **Docker Hub account** (to store Docker images)
- An **AWS account** (to provision cloud resources)

### 🛠️ GitHub Secrets
For secure access, you need to configure the following secrets in your GitHub repositor

