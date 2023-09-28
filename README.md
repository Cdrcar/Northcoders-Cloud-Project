# Cloud Engineering Team Project

## [Table of Contents](#table-of-contents)

- [Overview](#overview)
- [Objective](#objective)
- [Technologies Used](#technologies-used)
- [Infrastructure Overview](#infrastructure-overview)
- [CI CD](#ci-cd)
- [GitOps with ArgoCD](#gitops-with-argocd)
- [Monitoring and Metrics](#monitoring-and-Metrics)
- [Future Improvements](#future-improvements)
- [Presentation](#presentation)
- [License](#license)
- [Contact Me](#contact)

## [Overview](#overview)

This repository contains the infrastructure as code (IaC), configuration files, and documentation for the deployment of the Northcoders learner management system to AWS cloud. The project involved the deployment of both the frontend and backend applications, along with supporting services such as a container registry, Kubernetes cluster, and a relational database.

## [Objective](#objective)

The primary objective of this project was to deploy the learner management system and its supporting services to AWS cloud. The team aimed to leverage DevOps principles, automate CI/CD pipelines, and create a robust and scalable infrastructure.

## [Technologies Used](#technologies-used)

- AWS (Amazon Web Services)
- Terraform for Infrastructure as Code (IaC)
- Kubernetes (EKS - Elastic Kubernetes Service)
- Docker for containerization
- CircleCI for continuous integration and continuous deployment (CI/CD)
- ArgoCD for GitOps-based application deployment
- Prometheus and Grafana for monitoring and metrics

## [Infrastructure Overview](#infrastructure-overview)

### AWS Services Utilised

- **Amazon Elastic Container Registry (ECR):** Used for container image storage.
- **Elastic Kubernetes Service (EKS):** Managed Kubernetes cluster for container orchestration.
- **Amazon RDS (Relational Database Service):** A managed PostgreSQL database used by the backend.

### Infrastructure as Code (Terraform)

We used Terraform to provision and manage the AWS infrastructure. The IaC scripts are organized into modules and include:

- **VPC:** Virtual Private Cloud with both public and private subnets.
- **EKS Cluster:** Kubernetes cluster with node groups.
- **Security Groups:** Network security rules for resources.
- **RDS Instance:** PostgreSQL database with encryption.
- **Load Balancers:** For frontend and backend services.
- **IAM Roles and Policies:** For access control.

## [CI CD](#ci-cd)

- **CircleCI:** We set up automated CI/CD pipelines for both frontend and backend repositories on GitHub. These pipelines build, test, and deploy the applications.

## [GitOps with ArgoCD](#gitops-with-argocd)

- **ArgoCD:** We adopted a GitOps approach to application deployment using ArgoCD. Our Kubernetes manifests are stored in Git repositories, and ArgoCD ensures that the clusters reflect the desired state.

## [Monitoring and Metrics](#monitoring-and-metrics)

- **Prometheus and Grafana:** We implemented monitoring and metrics using Prometheus for data collection and Grafana for visualizing metrics through dashboards.


## [Future Improvements](#future-improvements)

We plan to improve in the future:

- Enhanced Monitoring: Implement more advanced alerting and anomaly detection.
- Security Enhancements: Implement stricter IAM roles and security policies.
- Scalability: Optimize the infrastructure for auto-scaling based on traffic.
- Backup and Disaster Recovery: Implement automated backup and recovery procedures.
- Apply other technologies like Jenkins.

## [How to Recreate the Environment](#how-to-recreate-the-environment)

To recreate this environment, follow the step-by-step instructions provided in the Instructions.md file. Ensure that you have the required AWS credentials, Terraform, kubectl, and other dependencies installed.

## [Presentation](#presentation)

For a visual overview and more details about this project, please refer to our presentation [link]().

## [Contact](#contact)

If you have any questions or need further information, feel free to reach out to our team:

- [Tom Wroe](https://github.com/Hyzad)
- [Carmela Rey](https://github.com/cdrcar)
- [Manal Abdulqawi](https://github.com/ManalAbdulqawi)
- [Luis Fifield](https://github.com/LouisFifield)

Thank you for your interest in our Cloud Engineering Team Project!
