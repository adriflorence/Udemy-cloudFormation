# Infrastructure as Code

Practice AWS CloudFormation script to roll out infrastructure.

## Components included:

- Web Server Instance

## Trigger stack creation:

``` aws cloudformation create-stack --stack-name udemy-test --region eu-west-1 --template-body file://stack.yaml ```