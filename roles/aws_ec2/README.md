# aws_ec2
Creates a single EC2 instance based on the inputs which are all found in the role defaults.

Creates an SSH key if the `aws_ec2_key_name` provided doesn't exist. 

Creates a Route 53 record for the instance based on its name if `aws_ec2_dns_zone` is provided.

Creates a Security Group which will have SSH/HTTPS 0.0.0.0/0 open unless modified.
