# Index
1. What is Networking ?
2. What is a VPC in AWS ?
3. 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# I. What is Networking ?
 - Virtual Private Cloud
 - Within each VPC, our compute instances (EC2) are hosted on subnets that we create in selected availability zones (AZs) within the AWS region we chose to operate within
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# II. Shared security model 
 - Security responsibilities are shared between:
    a. AWS Cloud Provider - responsible for building and securing its cloud infrastructure i.e. Security of the Cloud 
    b. AWS Customer - responsible to design acceptable security provisions for your applications and data hosted within the AWS cloud i.e. Security in the Cloud
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# II. What is a VPC in AWS ?
 - The networking layer at AWS
 - The official name of a VPC is an EC2-VPC
 - EC2 instances are usually hosted within a VPC
 - And within each VPC, our compute instances (EC2) are hosted on subnets that we create in selected availability zones (AZs) within the AWS region we chose to operate within
 - Each VPC is a logically isolated “data center” where your computer instances and various AWS services reside

## How is VPC a managed serivice ?
 - Although the VPC is a managed service, AWS customers make most of the choices and decisions on their own after AWS carries out the initial creation of the VPC
 - We generally work with networking services using the VPC console
    a. When we create a VPC, AWS’s job is securing our VPC as a private isolated software data center linked to our AWS account
    b. Within the VPC “toolbox” are many configurable options, including route tables, public and private subnets, VPN connections, gateways, and private endpoints
       A VPC toolbox is a large toolbox containing a variety of tools and attachments that you can mesh or cobble together any way they suit our needs
    c. There are multiple security choices available at every network level allowing you to fully protect your EC2 instances: security groups and network access control lists (ACLs)
    d. A VPC also has multiple connectivity options, allowing you to connect your VPC :
        1. To the Internet
        2. To our own private data center
        3. To other VPCs within our region or outside our region
        4. To other AWS accounts holders’ VPCs
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
