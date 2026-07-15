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

## Architecture Overview and Workflow Diagrams:

### Part 1: Launching a Kubenetes Cluster:

- Launch and Connect to an EC2 Instance:  
<img src="part1-workflow-diagrams/part1-workflow-diagram1.png" width="700">

- Launch EKS Cluster using eksctl (Error):  
<img src="part1-workflow-diagrams/part1-workflow-diagram2.png" width="700">

- Launch EKS Cluster with correct IAM role (Successful):  
<img src="part1-workflow-diagrams/part1-workflow-diagram3.png" width="700">

- Utilize CloudFormation to track creation of EKS cluster:  
<img src="part1-workflow-diagrams/part1-workflow-diagram4.png" width="700">

- Access EKS from the Management Console:  
<img src="part1-workflow-diagrams/part1-workflow-diagram5.png" width="700">

- Completed overview of Part1:  
<img src="part1-workflow-diagrams/part1-workflow-diagram6.png" width="700">

---

### Part 2: Setting up Kubernetes Deployment:

- EC2 and EKS setup from Part1:  
<img src="part2-workflow-diagrams/part2-workflow-diagram1.png" width="700">

- Pulling the code for the Backend from GitHub:  
<img src="part2-workflow-diagrams/part2-workflow-diagram2.png" width="700">

- Building container image for the backend:  
<img src="part2-workflow-diagrams/part2-workflow-diagram3.png" width="700">

- Pushing containter image to Amazon ECR:  
<img src="part2-workflow-diagrams/part2-workflow-diagram4.png" width="700">

- Completed overview of Part2:  
<img src="part2-workflow-diagrams/part2-workflow-diagram5.png" width="700">

---

### Part 3: Creating Kubernetes Manifests:

- EC2 and EKS setup from Part1:  
<img src="part3-workflow-diagrams/part3-workflow-diagram1.png" width="700">

- Pulling the Code from Part2:  
<img src="part3-workflow-diagrams/part3-workflow-diagram2.png" width="700">

- Building container image from Part2:  
<img src="part3-workflow-diagrams/part3-workflow-diagram3.png" width="700">

- Pushing to ECR from Part2:  
<img src="part3-workflow-diagrams/part3-workflow-diagram4.png" width="700">

- Setting up app for deployment by creating Manifests:  
<img src="part3-workflow-diagrams/part3-workflow-diagram5.png" width="700">

- Completed Overview of Part3:  
<img src="part3-workflow-diagrams/part3-workflow-diagram6.png" width="700">

---

## Technologies Used

- **Amazon EC2** – command workstation  
- **Amazon EKS** – Kubernetes control plane  
- **Amazon ECR** – container registry  
- **AWS IAM** – permissions and roles  
- **AWS CloudFormation** – infrastructure orchestration  
- **Docker** – containerization  
- **Kubernetes** – orchestration  
- **kubectl** – cluster interaction  
- **eksctl** – cluster provisioning  
- **Git & GitHub** – version control  

---