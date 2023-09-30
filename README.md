
# Setting Up a VPC with Subnets, EC2 Instances, Route Table, Internet Gateway, and Load Balancer on AWS

This guide will walk you through the process of creating a Virtual Private Cloud (VPC) on Amazon Web Services (AWS). Inside this VPC, we will create two subnets, launch two EC2 instances, set up a route table, associate an internet gateway for internet access, and configure a load balancer.


![image](https://github.com/krishwuds/CREATING-AWS-REASOURCES-USING-TERRAFORM/assets/143382092/08cc61bc-06ee-47c9-b1bd-5395e9277a97)



## Prerequisites

- [AWS CLI](https://aws.amazon.com/cli/)
- [Terraform](https://www.terraform.io/downloads.html)

## Step-by-Step Guide

### Step 1: Clone the Repository
```bash
git clone <repository_url>
cd <repository_directory>
```

### Step 2: Configure AWS Credentials
```bash
aws configure
```

### Step 3: Initialize Terraform
```bash
terraform init
```

### Step 4: Create a VPC Configuration
Edit your Terraform configuration file (e.g., `main.tf`) to define the VPC, subnets, EC2 instances, route table, internet gateway, and load balancer.

### Step 5: Plan and Apply
```bash
terraform plan
terraform apply
```

### Step 6: Verify the Setup
After Terraform provisioning is complete, verify the VPC, subnets, EC2 instances, route table, internet gateway, and load balancer creation using the AWS Management Console or Terraform outputs.

### Step 7: Access Your EC2 Instances
Use the public IP addresses or DNS names of your EC2 instances to access them over the internet.

### Step 8: Test Load Balancer
Ensure that the load balancer is working correctly by accessing it using its DNS name.

### Step 9: Clean Up (Optional)
If needed, run `terraform destroy` to remove the resources created by Terraform.

### Step 10: Commit and Push
```bash
git add .
git commit -m "Add Terraform configuration for VPC, subnets, EC2 instances, route table, internet gateway, and load balancer"
git push origin master
```

Feel free to customize this README with additional information, troubleshooting tips, or any other relevant details.
```

Replace `<repository_url>` and `<repository_directory>` with the actual URL and directory name of your GitHub repository. Customize the configuration in `main.tf` to match your specific requirements, such as choosing the appropriate AMIs, security group rules, and load balancer settings.
