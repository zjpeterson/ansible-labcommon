# ansible-labcommon
Common lab needs for different environments. On Galaxy as `zjpeterson.labcommon`.

## AWS Roles
### aws_vpc
Creates a simple VPC with an Internet Gateway and a single subnet attached to it. Most defaults are suitable but be sure to set `aws_vpc_region` if you don't want us-east-2.

The role sets `aws_ec2_region`, `aws_ec2_vpc`, and `aws_ec2_subnet` at the end for convenience if you are going to follow up with the `aws_ec2` role.

### aws_ec2
Creates a single EC2 instance based on the inputs which are all found in the role defaults.

Creates an SSH key if the `aws_ec2_key_name` provided doesn't exist. 

Creates a Route 53 record for the instance based on its name if `aws_ec2_dns_zone` is provided.

Creates a Security Group which will have SSH/HTTPS 0.0.0.0/0 open unless modified.
