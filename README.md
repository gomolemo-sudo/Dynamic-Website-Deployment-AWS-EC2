# Creating a Dynamic Website on AWS: Step-by-Step Guide  

## Introduction  
When building reliable and highly available applications on AWS, understanding how to architect secure, scalable, and cost-effective solutions is critical. In this guide, we’ll explore best practices and detailed steps to design architectures that ensure your workloads are both resilient and secure. We'll cover key AWS services, configurations, and strategies to help you optimize for performance, fault tolerance, and cost efficiency.
  
## Analyzing the Existing EC2 Instance
Before diving into the application deployment, it's crucial to review the EC2 instance settings. In this step, we explore the EC2 instance’s configuration, confirming whether it is in a public subnet, ensuring the right ports are open, and verifying its connection settings. This analysis lays the foundation for configuring and securing the instance in later steps.
![image](https://github.com/user-attachments/assets/efab563d-eef1-445c-9bbf-cd888313fa9b)


## Connecting to AWS Cloud9 IDE on the EC2 Instance
AWS Cloud9 offers a powerful, cloud-based IDE that directly integrates with EC2 instances. This environment allows you to edit files, execute code, and test changes without needing additional software or SSH access. By connecting to Cloud9, we create an efficient development space to work on the café’s application directly from the cloud.
![image](https://github.com/user-attachments/assets/db8372ad-0f3d-4476-853d-22255b18172b)


## Analyzing the LAMP Stack and Web Server Configuration
The LAMP stack (Linux, Apache, MySQL, PHP) is the core technology that powers the café’s dynamic website. In this step, we verify the proper installation and configuration of Apache, PHP, and MySQL. Ensuring that these components are working correctly is essential for the café’s website to run smoothly, providing both dynamic content and database connectivity.
![image](https://github.com/user-attachments/assets/2f60f4da-c5a2-4c00-92ca-ec43122e6cc7)


## Editing Web Server Files Using Cloud9
Cloud9’s file explorer makes it easy to manage the files necessary for running the café’s website. In this step, we configure the web server by creating an HTML test page, ensuring the server is properly serving content. This allows us to confirm that the web server is configured correctly before deploying the full application.
![image](https://github.com/user-attachments/assets/913cb943-832c-4076-ad9e-079e8ef0e370)


## Installing the Café Application
Once the server environment is prepared, the next step is to install the café's dynamic web application. By downloading the necessary application files and unzipping them directly into the /var/www/html/ directory, we ensure that the web server is ready to host the application and serve dynamic content to users.
![image](https://github.com/user-attachments/assets/370ac81a-3857-4b8a-8abc-bb62d83b8fd8)


## Configuring the MySQL Database for the Application
A functional MySQL database is key for storing user data, such as orders and customer information. In this step, we set up the MySQL database, run scripts to create the necessary tables, and confirm the café’s product data is stored correctly. This database setup is essential for the online ordering system to work seamlessly.
![image](https://github.com/user-attachments/assets/d55fd22c-cdf3-4754-b183-75fe1b0db7bb)


## Testing the Web Application
Testing the web application is critical to ensuring it functions as expected. After setting up the application and database, we navigate through the menu and place a test order. This ensures that users can browse products, and place orders and that those orders appear in the order history, confirming the application is operational.
![image](https://github.com/user-attachments/assets/71f375a8-1fdb-4c0c-8f20-856fca0b7f00)
![image](https://github.com/user-attachments/assets/7ad6e6ed-798d-44e6-b402-da179bcde2a8)


## Creating Development and Production Environments Across AWS Regions
Creating separate development and production environments across different AWS Regions improves application availability and scalability. In this step, we use Amazon EC2 to replicate the café’s website in a different region for better resilience and disaster recovery. The ability to scale and migrate between regions ensures the application can handle high traffic and be recovered in case of failure.
![image](https://github.com/user-attachments/assets/691b0ff8-39cb-4d85-89ba-5cd6589fee0b)


## Creating an AMI from the EC2 Instance
Amazon Machine Images (AMIs) allow you to create a snapshot of your EC2 instance, making it easy to launch new instances with the same configuration. By creating an AMI from the EC2 instance, we enable the possibility of replicating the setup in different regions, ensuring quick deployment and disaster recovery.



## Skills Demonstrated  
- LAMP Stack Deployment and Configuration  
- AWS EC2 Management and AMI Creation  
- MySQL Database Setup and Management  
- Multi-Region Architecture Design  
- Disaster Recovery Planning  
  

## Conclusion  
By completing this lab, you have learned how to deploy a dynamic website for a café using Amazon EC2, and you now have the ability to create scalable, highly available environments across AWS Regions. The ability to duplicate EC2 instances using AMIs for disaster recovery is a powerful tool for ensuring business continuity.

This architecture not only allows the café to accept online orders but also prepares the infrastructure to handle future scaling needs with minimal downtime. By utilizing AWS services like EC2, Cloud9, Systems Manager, and S3, we have created a resilient, scalable solution to meet both current and future business needs.


## Author  
**Gomolemo Hlatshwayo**  
- [LinkedIn](https://www.linkedin.com/in/lemon-paw)  
- [GitHub](https://github.com/lemon-paw)  
