# Discover Data Flow - AWS

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