# 🚀 Terraform AWS VPC + EC2 Project

This project demonstrates how to provision a **secure**, **scalable**, and **production-grade AWS environment** using **Terraform** from scratch.  
It is designed for those who want to move beyond tutorials and build **real-world Infrastructure as Code (IaC)** with **modular**, **clean**, and **automated provisioning**.

---

## 🧠 What You'll Learn

- Custom VPC creation (no default VPC)
- Public + Private Subnets across multiple AZs
- NAT Gateway and Internet Gateway setup
- Route Tables and associations
- EC2 instance provisioning in public subnet
- Sample `user-data.sh` for EC2 bootstrap
- Modular Terraform code structure
- AWS provider setup and Terraform CLI usage

---

## 🧰 Tech Stack

| Tool       | Purpose                              |
|------------|--------------------------------------|
| Terraform  | Infrastructure as Code (IaC)         |
| AWS EC2    | Virtual Server                       |
| AWS VPC    | Isolated Network                     |
| AWS IGW    | Internet access for public subnet    |
| AWS NAT    | Internet access for private subnet   |
| Amazon Linux | Lightweight base OS                |

---

## 📁 File Structure

```text
terraform-aws-vpc-ec2/
├── main.tf                  # Root module combining all resources
├── variables.tf             # Input variables
├── outputs.tf               # Exported output values
├── terraform.tfvars         # Variable values
├── nat.tf                   # NAT Gateway setup
├── private-subnet.tf        # Private subnets and route table
├── user-data.sh             # EC2 initialization script
└── README.md                # Project documentation
