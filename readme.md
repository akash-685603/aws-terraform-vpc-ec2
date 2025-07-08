🚀 Project Overview: Terraform VPC with EC2 Deployment
This project demonstrates the infrastructure-as-code (IaC) deployment of a fully functional AWS Virtual Private Cloud (VPC) along with public subnets and EC2 instances using Terraform.

🔧 What this project provisions:
✅ A custom VPC

✅ Two public subnets (in different Availability Zones)

✅ An Internet Gateway and appropriate route tables for public access

✅ A Security Group allowing SSH & HTTP access

✅ One or more EC2 instances inside public subnets

✅ Public IP auto-assignment to instances

📁 Folder Structure:
bash
Copy
Edit
Terraform_VPC_EC2/
├── main.tf             # Main resources: VPC, Subnets, IGW, EC2
├── provider.tf         # AWS provider config and region
├── variable.tf         # Input variables
├── terraform.tfvars    # Actual variable values
├── outputs.tf          # Useful outputs like instance public IP
├── .gitignore          # Files and folders to exclude from Git
📦 Prerequisites
Terraform installed (>= 1.0)

AWS CLI configured (aws configure)

A valid key pair name for EC2 access

Proper IAM permissions to create VPC and EC2 resources

🧪 Usage
bash
Copy
Edit
terraform init
terraform plan
terraform apply
After deployment, Terraform will output the public IP of your EC2 instance so you can SSH or access it in your browser (if web server is set up).

