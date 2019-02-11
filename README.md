# A Basic CloudFormation Stack for Testing

This CloudFormation template is a stripped down version of my other project, [A CloudFormation Template for Deploying an Ad-Blocking DNS Server](https://github.com/CloudEric/dnsvpn-cloudformation). This lays down a basic set of components that can be used for testing functionality of various systems.

A quick-create link can be found [here](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?stackName=teststack&templateURL=https://s3.amazonaws.com/clouderic.net/basic-stack-cloudformation.yaml)

---
## Included components
- VPC with a small subnet and Internet gateway
- A security group with forwarding for ssh, DNS, VPN, and web ports
- EC2 instance with the latest Amazon Linux 2 AMI
- EBS volume for docker bind mounts
- Docker
- Docker Compose

This project is only intended for testing and reference.
