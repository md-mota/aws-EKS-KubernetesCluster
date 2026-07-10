# AWS EKS Kubernetes Cluster Deployment

## Project Overview

This project demonstrates how to deploy a fully containerized backend application on **Amazon EKS (Elastic Kubernetes Service)** using AWS best practices.  
It follows a complete workflow from building the application image to deploying it on a Kubernetes cluster managed by EKS.

The project includes:

- Launching and configuring an EC2 instance  
- Creating an EKS cluster using `eksctl`  
- Building a Docker image for the backend  
- Storing the image in Amazon ECR  
- Creating Kubernetes Deployment and Service manifests  
- Deploying the backend using `kubectl`  

---