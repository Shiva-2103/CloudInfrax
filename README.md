# ☁️ CloudInfrax

CloudInfrax is a fully automated CI/CD pipeline setup to provision Amazon EKS (Elastic Kubernetes Service) clusters using **Terraform** and **Jenkins**.

---

## 🚀 Project Overview

This repository enables:

- Automated EKS provisioning with Terraform.
- Jenkins Pipeline integration for Infrastructure as Code (IaC) deployment.
- Basic AWS VPC, Subnet, IAM Roles, and Node Groups configuration.
- Modular and readable Terraform setup.

---

## 📂 Directory Structure
```
CloudInfrax/
├── eks/
│ ├── main.tf # Terraform infrastructure code
│ ├── variables.tf # Variable declarations (optional)
│ ├── outputs.tf # Output values (optional)
│ └── provider.tf # AWS provider setup
├── Jenkinsfile # Jenkins pipeline for EKS provisioning
```

---

## 🧰 Tools Used

- **Terraform**
- **Jenkins**
- **Amazon EKS**
- **IAM Roles & Policies**
- **AWS CLI**

---

## ⚙️ How to Run

> Make sure AWS credentials are configured in Jenkins before running.

### 1. Clone the Repository

```bash
git clone https://github.com/Shiva-2103/CloudInfrax.git
cd CloudInfrax/eks
```

2. Initialize Terraform
```bash
terraform init
```

3.  Plan & Apply Infrastructure
```bash
terraform plan
terraform apply 
```

4. Jenkins Setup
- Add your AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY in Jenkins credentials.

- Use the provided Jenkinsfile in your Jenkins Pipeline project.

- Trigger the pipeline to provision the EKS cluster.


### ✅ EKS Resources Created
- Custom VPC and Subnets

- IAM roles and policy attachments

- EKS Control Plane

- Managed Node Group


### Notes
- Ensure your AWS user has sufficient IAM permissions.

- Terraform version >=1.0.0 recommended.

- Compatible with AWS provider >=4.0.




