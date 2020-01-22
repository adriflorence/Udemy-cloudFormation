# Infrastructure as Code

Practice AWS CloudFormation script to roll out infrastructure.

## Components included in stack.yaml:

- EC2 Instance (Web Server)
- Web Server Security Group

## Trigger stack creation:

``` aws cloudformation create-stack --stack-name udemy-test --region eu-west-1 --template-body file://stack.yaml ```

## Trigger stack update:

``` aws cloudformation update-stack --stack-name udemy-test --region eu-west-1 --template-body file://stack.yaml ```

## Components included in activity-stack.yaml:

- VPC