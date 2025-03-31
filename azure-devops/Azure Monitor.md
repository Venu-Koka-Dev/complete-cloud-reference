# Index
1. What is Continuous Monitoring ?
2. What is Observability ?
3. What is Azure Monitor ?
4. What you can do with Azure Monitor ?
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# I. What is Continuous Monitoring ?
 - Monitoring is a crucial part of the DevOps process
 - It is recommended to incorporate monitoring because it helps you fully utilize the availability and performance of your applications and services
 - With continuous monitoring, release pipelines can include monitoring data from Application Insights and other Azure resources
 - When the release pipeline notices an Application Insights alert, the pipeline can roll back the deployment until the problem gets mitigated
 - If all checks pass in the pipeline, deployments can proceed instantly from test environments all the way to production, without needing manual intervention. 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# II. What is Observability ?
 - Three pillars of observability: these are the types of data that monitoring tools gather and investigate to provide adequate observability of a software application
    1. Metrics
    2. Logs
    3. Traces 
 - To conduct observability, collect data from numerous pillars and aggregate that data across the entire set of monitored resources
 - Azure Monitor keeps data from various sources, the data can be linked and investigated using the same tools
 
 # What is Azure Application Insights ?
 - Azure Application Insights is a tool that observes availability, performance, and use for web applications
 - Azure Pipelines integrates with Azure Application Insights to continuously monitor your DevOps release pipeline throughout the software development lifecycle
  
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# III. What is Azure Monitor?
 - Azure Monitor is not part of the Azure DevOps toolchain
 - Azure Monitor aids in maximizing your applications' availability and performance
 - It provides a complete solution for gathering and interpreting data from your application
 - This data helps you comprehend how your applications perform in production, and you can proactively recognize problems that need resolving.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# IV. What you can do with Azure Monitor ?
 1. Detect and analyze issues across applications and dependencies
 2. Correlate infrastructure problems with insights from the VMs and containers
 3. Create visualizations for logs and other kinds of telemetry

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
