# terraform-aws-vpc

# Terraform AWS VPC Module

This module creates:
- VPC
- Subnet

## 🚀 How to use

Do NOT change anything inside this repo.

Use this module from your main Terraform project like below:

```hcl
module "vpc" {
  source = "git::https://github.com/ganesh55655555/terraform-aws-vpc.git?ref=v1.0.0"

  vpc_cidr    = var.vpc_cidr
  subnet_cidr = var.subnet_cidr
  vpc_name    = var.vpc_name
}


📥 Variables (inputs)
Name	Description	Example
vpc_cidr	VPC CIDR block	10.0.0.0/16
subnet_cidr	Subnet CIDR	10.0.1.0/24
vpc_name	Name of VPC	demo-vpc


📤 Outputs
Name	Description
vpc_id	VPC ID
subnet_id	Subnet ID
📝 Example values (terraform.tfvars)
vpc_cidr    = "10.0.0.0/16"
subnet_cidr = "10.0.1.0/24"
vpc_name    = "demo-vpc"


