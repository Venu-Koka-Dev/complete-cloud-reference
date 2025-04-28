# Index
1. F
2. F
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### 1. B2C E-commerce website
 - Web application consists of dynamic content (such as products and their prices) and static content (such as the company logo)
 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Strategy 1: Simple straight forward Lift & Shift technique 
 - Migrating the Web application from On-prem to AWS Platform: just plain simple lift-and-shift strategy
![E-commerce web application on On premises Vs AWS](../assets/ecomm-onprem-aws.png)

 - We can use:
    a. VNets & subnets to separate systems with different security levels from each other i.e. by using access-control lists, she can control ingoing and outgoing traffic for each subnet

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Strategy 2: Improvising the architecture on AWS
![Full fledged architecture for E-commerce web application on AWS](../assets/full-ecomm-aws.png)

 - AWS Services used:
    a. CDN for delivering static content better performance
    b. Load balancer for high availability of VMs
    c. A managed database to decrease maintenance costs
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



