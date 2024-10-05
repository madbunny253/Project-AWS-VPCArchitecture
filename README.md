# Project-AWS-VPCArchitecture

**Design and Configure a VPC**
I created a VPC with custom IP ranges, ensuring a well-defined network structure. I set up both public and private subnets and configured route tables, associating them with the appropriate subnets for proper traffic management.

**Implement Network Security**
To secure the infrastructure, I implemented network access control lists (ACLs) to manage inbound and outbound traffic. I configured security groups for EC2 instances, specifying port and protocol rules to control access and protect the instances from unauthorized traffic.

**Provision EC2 Instances**
I launched EC2 instances in both public and private subnets. I set up security groups tailored to each instance's needs, allowing only the necessary traffic. I also created and assigned IAM roles with precise permissions to the instances, ensuring secure and restricted access to AWS resources.

**Networking and Routing**
To enable internet access, I configured an Internet Gateway for instances in the public subnet. I also set up a NAT Gateway to allow outbound internet access for private subnet instances. I then created and managed route tables, associating them with the appropriate subnets to ensure efficient and secure network routing.

**SSH Key Pair and Access Control**
I generated an SSH key pair, securely stored the private key, and configured EC2 instances to accept SSH connections using the key pair. I implemented strict IAM policies and roles to enforce access control, ensuring that only authorized users could access and manage AWS resources.

**Test and Validate the Setup**
After completing the setup, I successfully SSH'd into the EC2 instances using the private key and verified network connectivity between instances in different subnets. I tested and validated the security group rules and network ACL settings to ensure the environment was secure and functioning as expected.
