# aws_vpc
Creates a simple VPC with an Internet Gateway and a single subnet attached to it. Most defaults are suitable but be sure to set `aws_vpc_region` if you don't want us-east-2.

The role sets `aws_ec2_region`, `aws_ec2_vpc`, and `aws_ec2_subnet` at the end for convenience if you are going to follow up with the `aws_ec2` role.
