#  Expense Application Dev Infrastructure using Terraform

##  Project Overview
This project demonstrates Infrastructure as Code (IaC) implementation using Terraform to provision and manage the development environment for an Expense application.

The infrastructure is designed to support application deployment by creating core cloud resources such as networking, compute, and security components in a consistent and automated manner.

The setup follows industry best practices for environment isolation, scalability, and maintainability.

---

##  Objectives

- Provision application infrastructure using Terraform
- Maintain isolated development environment
- Automate infrastructure deployment
- Ensure consistency and repeatability
- Follow DevOps and IaC best practices

---

##  Tech Stack

- Infrastructure as Code: Terraform
- Language: HCL (HashiCorp Configuration Language)
- Cloud Platform: AWS
- Services:
  - VPC
  - EC2
  - Security Groups
  - Subnets
  - Internet Gateway
- Version Control: Git

---

##  Architecture

- Environment: Development (Dev)

### Infrastructure Components:
- VPC: Isolated network for application resources
- Subnets:
  - Public subnet (for external access)
  - Private subnet (for internal services)
- Internet Gateway: Enables outbound internet access
- Route Tables: Manage traffic routing
- EC2 Instances: Host application components
- Security Groups: Control inbound and outbound traffic

This architecture provides a secure and scalable foundation for deploying a multi-tier application.

---

##  Repository Structure
├── main.tf
├── variables.tf
├── outputs.tf
├── provider.tf
├── terraform.tfvars
└── README.md


---

##  Workflow

1. Define infrastructure configuration in Terraform
2. Initialize Terraform environment
3. Validate configuration files
4. Generate execution plan
5. Apply configuration to provision infrastructure
6. Maintain infrastructure state for updates

---

##  Key Features

- Environment-specific infrastructure (Dev)
- Declarative infrastructure definition
- Automated provisioning
- Scalable and reusable configuration
- Network and security setup included

---

##  Engineering Highlights

### Environment Isolation
Dedicated development environment ensures safe testing without impacting other environments.

### Automation
Infrastructure provisioning is fully automated, reducing manual effort.

### Consistency
Ensures identical infrastructure across deployments.

### Maintainability
Structured configuration improves readability and future scalability.

---

##  Execution Steps

### Initialize Terraform
```bash
terraform init

Validate Configuration
terraform validate
Plan Infrastructure
terraform plan
Apply Configuration
terraform apply
Destroy Infrastructure
terraform destroy


Real-World Use Cases
Setting up development environments for applications
Supporting CI/CD pipelines
Testing infrastructure changes safely
Standardizing infrastructure across teams


Challenges & Solutions
Challenge	Solution
Resource dependency issues	Managed using Terraform dependency graph
Environment isolation	Used dedicated dev configuration
Network configuration complexity	Structured VPC and subnet design
Security management	Implemented security groups


Future Enhancements
Add staging and production environments
Implement Terraform modules for reuse
Use remote backend (S3 + DynamoDB)
Integrate with CI/CD pipelines
Add monitoring and logging setup

Key Learnings
Terraform enables scalable infrastructure automation
Environment isolation is critical for safe deployments
Proper network and security configuration is essential
Infrastructure as Code improves consistency and reliability





