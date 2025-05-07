# Index
1. What is Wordpress ?
2. Architecture of a typical simple website developed using Wordpress
3. Migration strategies to AWS Cloud
4. Deploying & deleting using AWS CloudFormation
5. Deploying manually 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# I. What is Wordpress ?
 - WordPress is a content management system (CMS)
 - It allows us to create and manage websites easily without needing to write much code
 - It started as a blogging platform in 2003 but has since evolved into a full-featured system used for everything from personal blogs to large corporate websites and online stores
 - Key features:
    a. Easy-to-use Admin dashboard for managing posts, pages, media, and settings
    b. Thousands of themes and plugins to customize functionality and appearance
    c. Strong community support and frequent updates
    d. SEO-friendly out of the box
 - There are two main versions:
    a. WordPress.org: Free, open-source software you can install on your own web server. Gives you full control over customization, plugins, and themes
    b. WordPress.com: A hosted service with a more managed experience—great for beginners but with more limitations unless you pay for premium plans
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# II. Architecture of a typical simple website developed using Wordpress
![A typical MVC based Web App](../assets/wordpress-standard-mvc-architecture.png)

 - WordPress is built using a mix of widely-used web technologies
1. Programming Languages
    a. PHP: The primary server-side language WordPress is written in.
    b. JavaScript: Used for interactivity in the admin interface and themes. Modern WordPress also uses:
    c. React (in the block editor, aka Gutenberg)
    d. HTML/CSS: For structure and styling of front-end themes and admin UI.

2. Database
    a. MySQL or MariaDB: Stores all site content, user information, settings, etc.

3. Web Server
   Typically runs on:
    a. Apache (most common)
    b. Nginx (lighter alternative)
   Compatible with most other web servers.

4. CMS Architecture
    a. Themes: Control the look and layout of the site.
    b. Plugins: Extend functionality (e.g., SEO, e-commerce, security).
    c. REST API: Enables communication with other apps and services.

5. Admin Interface
    a. Built with a mix of PHP, JavaScript (including React), and AJAX for dynamic features.

6. Hosting Environment
    a. Runs on a LAMP stack (Linux, Apache, MySQL, PHP), but works with many other configurations like LEMP (Nginx instead of Apache)
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# III. Migration strategies to AWS Cloud 
1. Lift & Shift strategy
    - Simple & quick: using EC2 instances & DB server
    - Not cost-effective & not performant

2. Optimal utilization of features that AWS has to offer
    - Using various services of AWS      
       a. Elastic Compute Cloud (EC2)                   - IaaS service to create a Linux virtual machine with an optimized distribution called Amazon Linux to install Apache, PHP, and WordPress
       b. Elastic Load Balancing (ELB)                  - IaaS service using a type of Application Load Balancer (ALB), which operates on layer 7 (HTTP and HTTPS) & distributes traffic to a bunch of virtual machines and is highly available by default
       c. Relational Database Service (RDS) for MySQL   - PaaS service using which we choose the database type & size (storage, CPU, RAM), and RDS takes over operating tasks like creating backups and installing patches and updates
       d. Elastic File System (EFS)                     - PaaS service to provides a scalable, highly available, and durable network filesystem using the NFSv4.1 protocol
       e. Security groups                               - IaaS service a firewall service to control incoming and outgoing traffic to your virtual machine, your database, or your load balancer
       f. AWS CloudFormation                            - an IaC service 

![AWS MVC Wordpress Architecture](../assets/aws-mvc-wordpress-architecture.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# IV. Deploying & deleting using AWS CloudFormation
 - AWS CloudFormation is a tool provided by AWS for free
 - Creating a cloud infrastructure for WordPress and any other application can be fully automated.

In AWS management console -> Search: CloudFormation -> Create Stack 
-> Select: Choose an existing template -> Template source: Amazon S3 URL
-> Amazon S3 URL: https://s3.amazonaws.com/awsinaction-code3/chapter02/template.yaml
-> Next
-> Stack name: Wp-blog-app -> WordpressAdminPassword: Admin12wp
-> Add Tag: Purpose: Learning 
-> Next
-> Create Stack
-> After completion: Click on URL to open the Wordpress Website


(Optional) Deleting a deployment
In AWS management console -> Search: CloudFormation -> Select the Stack name: Wp-blog-app -> Delete 

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# V. Deploying manually 

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------








