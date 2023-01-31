# Discover Data Flow - AWS

![image](https://user-images.githubusercontent.com/29733103/215833042-a3afa617-9126-4647-a8f2-d9ee81244f90.png)

## Assume Role
The CrowdStrike Discover service assumes the role provisioned during account registration.
  
## Read-Only API Calls
Using STS temporary credentials, Discover performs the following API calls:
- "ec2:DescribeInstances"
- "ec2:DescribeImages"
- "ec2:DescribeNetworkInterfaces"
- "ec2:DescribeVolumes"
- "ec2:DescribeVpcs"
- "ec2:DescribeRegions"
- "ec2:DescribeSubnets"
- "ec2:DescribeNetworkAcls"
- "ec2:DescribeSecurityGroups"
- "iam:ListAccountAliases"
- "organizations:ListAccounts" (if using Organization Registration)
  
## EC2 & IAM Data Returned
