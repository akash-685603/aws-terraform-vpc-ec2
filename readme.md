# 🚀 Terraform VPC with EC2 Deployment

Welcome to the **Infrastructure-as-Code (IaC)** world! This project demonstrates how to deploy a complete AWS Virtual Private Cloud (VPC) setup with EC2 instances using **Terraform**.

---

## 🌐 Project Overview

Using this project, you'll provision a secure, internet-accessible infrastructure on AWS, including:

- ✅ A custom VPC
- ✅ Two public subnets across different Availability Zones
- ✅ An Internet Gateway with proper route tables
- ✅ A Security Group allowing **SSH (port 22)** and **HTTP (port 80)** access
- ✅ One or more EC2 instances within public subnets
- ✅ Auto-assigned public IPs for EC2 instances

> Ideal for DevOps beginners, AWS learners, or anyone looking to practice Terraform in real-world scenarios.

---

## 📁 Folder Structure
Terraform_VPC_EC2/
├── main.tf # Main resources: VPC, Subnets, IGW, EC2
├── provider.tf # AWS provider config and region
├── variable.tf # Input variables declaration
├── terraform.tfvars # Values for variables (region, AMI, etc.)
├── outputs.tf # Outputs like EC2 public IP
├── .gitignore # Ignore Terraform state & sensitive files

---

## 📦 Prerequisites

Before you begin, make sure you have the following:

- ✅ [Terraform](https://www.terraform.io/downloads) installed (v1.0 or higher)
- ✅ AWS CLI installed and configured:  
  ```bash
  aws configure

🧪 Usage
Step-by-step Commands
# Initialize the project
terraform init

# Preview the execution plan
terraform plan

# Deploy infrastructure to AWS
terraform apply

At the end of the deployment, Terraform will print the public IP address of the EC2 instance.

🔗 You can use this IP to:

SSH into your instance

Or visit in the browser (if you install a web server like NGINX or Apache)

🧹 Cleanup
To destroy all the resources created:
terraform destroy

🙌 Contributing
Feel free to fork this repo, improve it, or raise issues. Learning and sharing is part of DevOps culture!

🧑‍💻 Author
Akash
DevOps Enthusiast | AWS Learner | Automation Explorer
📫 Feel free to connect on LinkedIn

🌟 If you found this helpful, give it a ⭐ on GitHub!


