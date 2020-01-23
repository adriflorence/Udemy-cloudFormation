# Infrastructure as Code

Practice AWS CloudFormation script to roll out infrastructure as code. This repository contains two files:

## 1. stack.yaml

### Components included in stack.yaml:

- EC2 Instance (Web Server)
- Web Server Security Group

### Trigger stack creation:

``` aws cloudformation create-stack --stack-name udemy-test --region eu-west-1 --template-body file://stack.yaml ```

### Trigger stack update:

``` aws cloudformation update-stack --stack-name udemy-test --region eu-west-1 --template-body file://stack.yaml ```

## 2. activity-stack.yaml:

### Components included in stack.yaml:

- VPC
- Public Subnet (x1)
- Route Table associated with the Subnet (x1)
- Internet Gateway attached to the VPC (x1) + Attachment
- Internet Route
- EC2 instance in the Public Subnet (x1)
- Security Group with Ingress rule attached to EC2 instance

## Tasks

Roll out infrastructure as code as per the requirements

Test whether EC2 instance is reachable publicly:

``` ping -c 4 <IP ADDRESS HERE> ```