# Application-Deployment



Application Deployment Project



Overview

This project demonstrates deployment of a React application using Docker, Terraform, Kubernetes and Jenkins CI/CD concepts.



Repository Used:

https://github.com/Vennilavangui/Trend.git



1)Application Deployment

Cloned the application repository.

Built the application using Docker.

Verified application deployment on AWS EC2.

Application accessible through EC2 public IP.



2)Docker

Created Dockerfile.

Built Docker image.

Pushed image to DockerHub.



3)Docker Image:

sandhyamanikanta/trend-app:v1



4)Terraform

Created Terraform configuration files for:

Security Group

EC2 Instance

Outputs

Variables



5)Files:

main.tf

outputs.tf

variables.tf



6)Kubernetes

Created:

deployment.yaml

service.yaml



7)Deployment uses Docker image:

sandhyamanikanta/trend-app:v1



8)Service Type:

LoadBalancer



9)Jenkins Pipeline

Created Jenkinsfile with stages:

1\. Checkout

2\. Build Docker Image

3\. Push Docker Image

4\. Deploy Kubernetes



10)Screenshots Included

Docker installation

Docker image build

Docker container running

Application running on EC2

Terraform init

Terraform validate

Kubernetes YAML creation

GitHub repository push



11)Tools Used

AWS EC2

Docker

DockerHub

Terraform

Kubernetes

Jenkins

GitHub



\#Author

Sandhya Krishna

