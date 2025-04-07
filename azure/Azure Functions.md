# Index
1. What is Serverless Computing ?
2. F
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# I. What is Serverless Computing ?
 - Function as a Service and Backend as a Service
 - Serverless is a method of computing where backend services are provided by a cloud service provider i.e. “less” in this term means the servers and underlying infrastructure are abstracted
 - Responsibilities in serverless computing:
    1. Cloud Service Provider: manages the infrastructure (server infrastructure, operating system, and other lower-level components) and automatically provisions and scales resources as needed  
    2. Cloud Service Consumers (Developers) : focus solely on writing code for their applications
 - Consumption pricing models where the users are charged on usage and execution

## Difference between Serverless Computing Vs BaaS Vs FaaS 
 - Serverless computing is related to BaaS and FaaS
 - They all provide an abstraction layer between the developer and the underlying infrastructure
 - However, they differ regarding the level of abstraction and the services provided


## Different Serverless solutions in Azure
1. Azure serverless compute services for applications
    a. Azure Functions
    b. Azure Logic Apps
    c. Azure Event Grid
    d. Azure Event Hubs

2. Serverless containers
    a.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# (FaaS) Functions as a Service in Azure
 - Level of abstraction is less, as the developers will still have to create the backend application logic
 - This code is executed in stateless compute instances managed by the cloud provider
 - FaaS provides an event-driven computing architecture where a specific event, such as message queues, HTTP requests, etc., can trigger a function
