Application Deployment Project

Overview

This project demonstrates the deployment of the Trend web application using Docker, Terraform, Jenkins, Kubernetes (Amazon EKS), and Docker Hub with an automated CI/CD pipeline.

---

Repository Used

Original Repository:
https://github.com/Vennilavanguvi/Trend.git

Project Repository:
https://github.com/sandhyaam13-prog/Application-Deployment

---

Architecture

GitHub
↓
Jenkins
↓
Docker Build
↓
Docker Hub
↓
Amazon EKS
↓
Kubernetes Deployment
↓
AWS LoadBalancer
↓
Live Application

---

1. Application Deployment

- Cloned the Trend application repository.
- Dockerized the application.
- Built the Docker image.
- Deployed the application to Amazon EKS.
- Exposed the application using Kubernetes LoadBalancer.
- Successfully verified the application through the LoadBalancer URL.

---

2. Docker

- Created Dockerfile.
- Built Docker image.
- Tagged Docker image.
- Pushed Docker image to Docker Hub.

Docker Image:

sandhyamanikanta/trend-app:v1

---

3. Terraform

Created Terraform configuration files for:

- EC2 Instance
- Security Group
- Variables
- Outputs

Files:

- main.tf
- variables.tf
- outputs.tf

Executed:

- terraform init
- terraform validate
- terraform plan
- terraform apply

---

4. Kubernetes

Created:

- deployment.yaml
- service.yaml

Deployment Image:

sandhyamanikanta/trend-app:v1

Service Type:

LoadBalancer

Successfully deployed application on Amazon EKS.

---

5. Jenkins CI/CD Pipeline

Created a Declarative Jenkins Pipeline with the following stages:

1. Checkout Source Code
2. Build Docker Image
3. Push Docker Image to Docker Hub
4. Deploy Application to Kubernetes

Integrated Jenkins with GitHub using Webhooks for automatic build on every push.

---

6. Docker Hub Repository

Repository:

sandhyamanikanta/trend-app

Image:

sandhyamanikanta/trend-app:v1

---

7. Tools Used

- AWS EC2
- Amazon EKS
- Docker
- Docker Hub
- Terraform
- Kubernetes
- Jenkins
- GitHub

---

8. Screenshots

Include screenshots of:

- Terraform init
- Terraform apply
- Docker image build
- Docker Hub repository
- Jenkins pipeline success
- kubectl get nodes
- kubectl get pods
- kubectl get svc
- Application running
- GitHub repository

- read me added for webhook

---

Author

Sandhya M
