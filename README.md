# terraform-aws-basic-web-deployment
## AWS Web Infrastructure with Terraform
**This project deploys a basic web infrastructure on AWS using Terraform. It includes a VPC with two public subnets, an Application Load Balancer (ALB), and two EC2 instances configured to serve as web servers. An S3 bucket is also created for general storage.**
### Project Structure
VPC and Subnets: Sets up a VPC with two public subnets across Availability Zones.
Internet Gateway and Route Table: Enables internet access for resources in the VPC.
Security Group: Allows HTTP (port 80) and SSH (port 22) access.
EC2 Instances: Deploys two EC2 instances in separate subnets, configured with user data scripts.
Application Load Balancer (ALB): Balances traffic between EC2 instances for high availability.
Target Group and Listener: Manages traffic routing and health checks for EC2 instances.
S3 Bucket: Provides storage with a unique bucket name.


### Prerequisites
**Terraform installed**

**AWS CLI configured with appropriate credentials**

**An AWS account with permissions to create resources**

### usage

Initialize Terraform:

**terraform init**

view the plan of the configration:

**terraform plan**

Apply the configuration:

 **terraform apply**
 
To delete all resources, run:

 **terraform destroy**
