AWS Security


## AWS Security Groups and NACL

AWS security groups and network access control lists (NACLs) are two essential tools for securing your resources in the Amazon Web Services (AWS) cloud. Security groups act as virtual firewalls, allowing you to control the inbound and outbound traffic to your instances. NACLs, on the other hand, are used to control traffic at the subnet level.

## Security Groups

Security groups are associated with individual EC2 instances or groups of instances. They allow you to specify which IP addresses or security groups are allowed to access your instances. You can create multiple security groups and apply them to different instances or groups of instances, giving you granular control over network access.

## NACLs

NACLs are associated with subnets and apply to all instances within that subnet. They allow you to control which traffic is allowed to enter or leave the subnet. NACLs are stateless, meaning that they do not track the state of connections. This can be advantageous in some cases, but it also means that you need to be careful when configuring NACLs to avoid accidentally blocking legitimate traffic.

## Using Security Groups and NACLs Together

Security groups and NACLs can be used together to provide multiple layers of security for your AWS resources. Security groups can be used to control traffic at the instance level, while NACLs can be used to control traffic at the subnet level. This allows you to create a defense-in-depth strategy that makes it more difficult for attackers to compromise your resources.


[Security Groups Reading](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-groups.html)

[NACL Reading](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)
