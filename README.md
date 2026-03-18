# Production Grade AWS EKS Cluster using Terraform

## Steps

### 1. Install Tools
- Terraform
- AWS CLI
- kubectl

### 2. Configure AWS
aws configure

### 3. Initialize Terraform
terraform init

### 4. Plan
terraform plan

### 5. Apply
terraform apply

### 6. Configure kubectl
aws eks update-kubeconfig --region ap-south-1 --name prod-eks-cluster

### 7. Verify
kubectl get nodes

## Architecture
- VPC with public & private subnets
- NAT Gateway
- EKS Cluster
- Managed Node Group

## Destroy
terraform destroy