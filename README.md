# 3-Tier-Web-architecture

![image](https://github.com/AjayAjex/3-Tier-Web-architecture/assets/106955998/ce5947cf-4893-484f-9b0d-c979bf71c1d5)



**Project Name: AWS Three-Tier Web Architecture**

The AWS Three-Tier Web Architecture is based on a software design pattern that divides the application into three interconnected tiers: the Presentation Tier, the Application (or Logic) Tier, and the Data Tier.

**Presentation Tier (UI Layer):**
This topmost layer directly interacts with users, managing the user interface.

**Application Tier (Logic Tier):**
Also known as the logic or middle tier, it houses the core business logic, processes user requests, communicates with the database, and handles application-specific tasks.

**Data Tier (Database Tier):**
Responsible for storing and managing data, including databases and data storage systems, this tier stores and retrieves information as requested by the application tier.

**Advantages/Reasons for Implementing Three-Tier Architecture:**

**Scalability:**
By separating the application logic, presentation, and data layers, each tier can be scaled independently, enabling resource allocation where needed during traffic surges.

**Maintainability:**
Dividing the application into layers simplifies management and maintenance. Changes in one tier don't impact the others, enhancing debugging, testing, and future enhancements.

**Security:**
Adding an extra layer of security by placing the data tier behind the application tier, ensuring controlled access to the database and shielding sensitive data from direct exposure.

**Reusability:**
Three-tier architecture promotes reusability, enabling components in one layer to be used in different parts of the application.

**Reasons Against Two-Tier Architecture:**
Two-tier architecture combines the presentation and application tiers, leading to limitations in scalability, maintainability, and security. Three-tier architecture offers flexibility, adaptability, and robustness, making it the preferred choice for modern web applications.

**Project Overview:**
I've developed a robust three-tier web architecture, providing a resilient foundation for hosting web applications with a focus on high availability, scalability, and security.

**Key Project Steps:**

Established a secure foundation with an S3 bucket for code storage and IAM roles for streamlined instance management.
Designed a VPC environment, strategically segmenting it into public and private subnets for web, app, and database tiers.
Implemented route tables, internet gateways, and NAT gateways for secure internet access.
Enhanced security with security groups for EC2 instances, databases, and load balancers.
Ensured multi-Availability Zone (AZ) redundancy for data durability and availability in the database layer.
Configured Nginx, Node.js, and React.js for the app and web tiers to optimize performance.
Integrated load balancing mechanisms, utilizing an Application Load Balancer (ALB) for web traffic, conducting health checks, and establishing auto-scaling groups for dynamic resource adjustments.
This comprehensive architecture not only provides a highly reliable environment for hosting web applications but also offers the scalability required to accommodate increased workloads, making it an ideal solution for web hosting on AWS.
