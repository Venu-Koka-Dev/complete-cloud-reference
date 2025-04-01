# Index
1. What is CI/CD ?
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# I. Continuous integration and continuous delivery (CI/CD)
 - IT professionals can automate all aspects of the DevOps process through Continuous Integration (CI) and Continuous Delivery (CD), with the option for Continuous Deployment as an additional step
 - These practices serve as the foundation for modern software development, ensuring efficiency, reliability, and speed in the delivery of applications
 - In summary:
    a. Continuous Integration involves automatically building and testing code with each commit to ensure that the software is always ready for release
    b. Continuous Delivery automates the process leading up to the release but still requires manual triggering for deployment
    c. Continuous Deployment takes it a step further by automatically deploying every change to production, eliminating the need for manual intervention in the release process

# What is Continuous Integration ?
 - Continuous Integration (CI) is a technique employed during the application development phase
 - It involves automatically building and testing code whenever a change is made to the main branch, ensuring seamless integration of new code changes with the existing codebase
 - To quickly identify and resolve integration errors, thereby maintaining software quality and enabling development teams to deliver software at a faster and more dependable pace
 - When modifications are made to the primary branch i.e. main branch, they undergo automatic validation
 - This validation process involves:
    a. Compiling the code to identify any errors and
    b. Conducting automated tests to ensure that the changes do not disrupt or degrade the application
 - Once the validation is successful, the code can be built and optionally packaged into a deployable artifact
 - This artifact represents a version of the code that can be transferred to different environments for further testing or release

# What is Continuous Delivery ?
 - Continuous Delivery (CD) builds upon Continuous Integration (CI) by automating the deployment of applications to specific environments, such as TEST or STAGING(DEV) environments but not PRODUCTION
 - CD streamlines the necessary steps for deploying a build artifact to these environments, allowing teams to verify that their application can be deployed at any given time
 - However, unlike Continuous Deployment, Continuous Delivery does not automatically deploy the application to production
 - Instead, it prepares all the required deployment steps so that the release to production can be easily triggered manually, for example, by pressing a button
 - This approach grants teams’ greater control over the timing and manner of changes being released

# What is Continuous Deployment ?
 - Continuous Deployment is an extension of Continuous Delivery that automates the deployment of applications to PRODUCTION without the need for manual intervention
 - With Continuous Deployment, any change that successfully passes through all stages of the production pipeline is automatically released to customers.
 - This allows for a quick feedback loop with end users
 - Continuous Deployment is particularly beneficial for teams that have confidence in their testing and release processes and want to speed up the release cycle even more.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
