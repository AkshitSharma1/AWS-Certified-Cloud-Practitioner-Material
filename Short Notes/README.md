# AWS Certified Cloud Practitioner Exam Short Notes
You can connect with me on- [![GitHub Follow](https://img.shields.io/github/followers/akshitsharma1?label=akshitsharma1&style=plastic&logo=github&color=green)](https://github.com/akshitsharma1)   [![LinkedIn Badge](https://img.shields.io/badge/akshitsharma1-LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/akshitsharma1/)

Happy learning!

## Deployment Models for Cloud Computing

- **Cloud-Hosted Deployment**  
  Run your applications on infrastructure managed by a cloud provider. This model offers rapid scalability, high availability, and removes the burden of maintaining physical hardware. It is ideal for dynamic workloads and businesses that require quick global expansion.

- **On-Premises Deployment**  
  Host your workloads on hardware located in your own data center. This model gives you complete control over your infrastructure and is often used when strict regulatory or compliance requirements necessitate local data control.

- **Hybrid Deployment**  
  Combine both cloud-based and on-premises resources for flexible operations. Hybrid solutions allow organizations to leverage the benefits of the cloud while maintaining legacy systems or sensitive data on-premises, creating a balanced approach that caters to diverse workload needs.

---

## Benefits of Cloud Computing

- **Shifting from Capital Expense (CAPEX) to Operational Expense (OPEX)**  
  Rather than investing heavily in physical infrastructure upfront, you pay for computing power as you use it. This enables spending only on consumed resources without committing large amounts of capital. It also offers the advantage of predictable monthly costs and improved budgeting flexibility.

- **Eliminating the Cost of Data Center Management**  
  Focus your efforts on core business projects instead of managing the physical aspects of servers, storage, and networking. By offloading routine maintenance and infrastructure management to the cloud provider, your team can concentrate on innovation and strategic initiatives.

- **Eliminating Capacity Guesswork**  
  Cloud platforms automatically adjust to your capacity needs. Instead of overprovisioning or struggling with undercapacity, you can quickly scale resources to match demand. This elasticity is especially useful during sudden traffic spikes or seasonal variations.

- **Leveraging Massive Economies of Scale**  
  Cloud providers aggregate usage across many customers, reducing costs through bulk purchasing and efficient resource utilization. This results in lower per-unit costs compared to what organizations would typically achieve on their own.

- **Boosting Speed and Agility**  
  New IT resources become available almost instantly via self-service, shortening the time from idea to deployment and facilitating rapid innovation. This agility enables faster testing, deployment, and iterative improvements of applications.

- **Global Deployment in Minutes**  
  Deploy applications across multiple regions worldwide with just a few clicks, improving latency and user experience with minimal extra cost. This is essential for companies with a global customer base, as it ensures low-latency interactions and compliance with regional data regulations.

---

## AWS Cloud Design Principles

- **Treat Operations as Code**  
  Automate infrastructure and configuration management using scripts and templates. This approach leads to reproducible environments and faster deployments, reducing the likelihood of human error.

- **Implement Frequent, Small, Reversible Changes**  
  Adopt an incremental approach to updates, which minimizes risk and simplifies rollback if needed. This practice supports continuous integration and continuous delivery (CI/CD) processes.

- **Continuously Refine Operational Procedures**  
  Regularly review and enhance your deployment and management processes to adapt to new challenges and technologies. This iterative improvement ensures that your operational practices remain effective over time.

- **Anticipate Failures**  
  Design systems with the expectation of component failures and ensure recovery strategies are in place. This proactive mindset leads to robust architectures that can withstand unexpected disruptions.

- **Learn from Operational Failures**  
  Analyze incidents to improve future resilience and performance. Documenting and understanding failures helps teams build more resilient systems and adopt best practices for future deployments.

---

## AWS Shared Responsibility Model

AWS divides security responsibilities between the provider and the customer. AWS manages the security *of* the cloud (hardware, software, networking, and facilities), while customers are responsible for security *in* the cloud (data, applications, and configurations).

---

## Amazon EC2 Instance Types

- **General Purpose Instances**  
  Offer balanced compute, memory, and network resources—ideal for web servers, development environments, and medium-sized databases. They provide versatility for a wide range of applications.

- **Compute-Optimized Instances**  
  Provide high CPU-to-memory ratios for compute-bound tasks like scientific simulations, batch processing, or gaming servers. They are engineered for high-performance computations and intensive processing tasks.

- **Memory-Optimized Instances**  
  Tailored for applications requiring large amounts of in-memory data processing, such as in-memory databases and real-time analytics. These instances support workloads that benefit from large memory sizes.

- **Accelerated Computing Instances**  
  Equipped with hardware accelerators (GPUs, FPGAs) for machine learning, video processing, and high-performance computing tasks. They deliver significant speedups for parallel processing and specialized computational workloads.

- **Storage-Optimized Instances**  
  Designed for applications that need high, sequential read/write throughput such as distributed file systems and data warehousing solutions. They are optimized for heavy data transfer operations and storage-intensive applications.

---

## AWS EC2 Instance Store

An instance store provides temporary block-level storage directly attached to the host machine. This ephemeral storage is best used for transient data—such as caches, buffers, or scratch files—that do not need to persist if the instance stops or terminates. It is crucial for workloads that require fast, temporary storage without the overhead of data durability.

---

## Amazon EC2 Pricing Options

### On-Demand Instances
- Ideal for short-term, unpredictable workloads.
- No upfront cost or long-term commitment; you pay only for the time you use.

### Reserved Instances
- **Standard Reserved Instances:** Provide significant discounts for committed usage over a fixed term.
- **Convertible Reserved Instances:** Allow you to change instance attributes while still receiving a discount, offering flexibility as your workload evolves.

### EC2 Instance Savings Plans
- Offer flexible commitment terms (1-year or 3-year) across instance families and regions.
- Provide savings in exchange for committing to a specific spend over a period, making it easier to predict long-term costs.

### Spot Instances
- Leverage spare capacity at up to a 90% discount.
- Suitable for fault-tolerant or flexible workloads, as these instances can be interrupted with little warning, making them ideal for batch jobs and data analysis tasks.

### Dedicated Hosts
- Provide physical servers dedicated to your use.
- Allow you to meet compliance requirements and control instance placement, with predictable costs and the ability to use existing server-bound licenses.

---

## Pricing Models for EC2

| Pricing Model          | Description                                          | Use Case                            | Key Features                                     |
| ---------------------- | ---------------------------------------------------- | ----------------------------------- | ------------------------------------------------ |
| **On-Demand**          | Pay for compute capacity by the hour or second       | Short-term, unpredictable usage     | No upfront commitment, flexible pricing          |
| **Reserved Instances** | Commit to using AWS resources for a 1 or 3-year term | Long-term, predictable usage        | Significant discounts, capacity reservation      |
| **Spot Instances**     | Bid for unused EC2 capacity                          | Cost savings for flexible tasks     | Potential cost savings, interruptions possible   |
| **Savings Plans**      | Flexible pricing model for various AWS services      | Commit to a certain amount of usage | Discounts over on-demand pricing, flexible usage |

---

## AWS Services Overview

- **AWS Management Console:**  
  A browser-based interface that simplifies resource management through an organized, graphical dashboard.

- **AWS Command Line Interface (CLI):**  
  Offers direct command access to AWS services, ideal for scripting and automation.

- **AWS Software Development Kit (SDK):**  
  Provides language-specific libraries and tools to integrate AWS services directly into your applications.

---

## AWS Cloud9

AWS Cloud9 is a browser-accessible integrated development environment (IDE) that allows you to write, run, and debug code in the cloud. It integrates seamlessly with AWS services and supports real-time collaboration.

---

## Virtual Private Cloud (VPC) Components

- **Internet Gateway (IGW):**  
  Connects your VPC to the internet, allowing instances in public subnets to send and receive traffic.

- **Virtual Private Gateway (VGW):**  
  Serves as the endpoint for VPN connections or AWS Direct Connect, linking your VPC to on-premises networks.

- **VPC Peering:**  
  Establishes private connectivity between two VPCs, even across different AWS accounts, for high-speed, secure data exchange without using the public internet.

- **AWS Direct Connect:**  
  Provides a dedicated network connection between your data center and AWS, bypassing the public internet for more consistent performance and potentially lower costs.

- **NAT Gateway:**  
  Enables instances in private subnets to access the internet for updates or patches while preventing direct inbound access.

- **NAT Gateway vs. NAT Instance:**  
  NAT Gateways are managed by AWS, offering easier scalability and maintenance, whereas NAT Instances are user-managed virtual machines that provide more configuration flexibility.

---

## Subnets

- **Private Subnet:**  
  A subnet without direct internet access, ideal for hosting resources that require enhanced security or internal communication.

- **Public Subnet:**  
  A subnet that is accessible from the internet, perfect for resources such as web servers that need to interact with external users.

---

## Security Groups and Network ACLs

### Security Groups
- Operate at the instance level.
- Provide stateful filtering that automatically tracks connection state.
- Allow only permit rules without the need for rule numbering.
- Enable dynamic updates and can specify sources by IP addresses, ranges, or security group IDs.

### Network ACLs (NACLs)
- Function as subnet-level firewalls.
- Are stateless, requiring separate inbound and outbound rules.
- Process rules in numerical order and support both allow and deny rules.

---

## Amazon Elastic Block Store (EBS)

EBS offers persistent block-level storage for EC2 instances. It provides various volume types optimized for different performance needs, automatic replication for durability, and snapshot capabilities for backups. Volumes can be resized as needed, and pricing depends on volume type, snapshot frequency, and data transfer.

---

## Amazon Elastic File System (EFS)

EFS is a scalable, fully managed file storage service that supports concurrent access by multiple EC2 instances. It automatically scales and provides high durability by replicating data across Availability Zones, making it ideal for shared file storage applications.

---

## Amazon S3 Storage Classes

| Feature                      | S3 Standard                                          | S3 Intelligent-Tiering                                                         | S3 Standard-IA                                         | S3 One Zone-IA                                                  | S3 Glacier                                                 | S3 Glacier Deep Archive                              |
| ---------------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------ | ------------------------------------------------------ | --------------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------- |
| **Description**              | General-purpose storage for frequently accessed data | Automatically moves data to the most cost-effective access tier based on usage | Infrequently accessed data, but rapid retrieval needed | Infrequently accessed data stored in a single availability zone | Long-term archive with retrieval times in minutes to hours | Lowest-cost storage for data that is rarely accessed |
| **Retrieval Time**           | Milliseconds                                         | Milliseconds                                                                   | Milliseconds                                           | Milliseconds                                                    | Minutes to hours                                           | Up to 12 hours                                       |
| **Use Cases**                | Frequently accessed data, low-latency needs          | Data with unknown or changing access patterns                                  | Infrequent access but needs quick retrieval            | Infrequently accessed, non-critical data                        | Archival data that doesn't require immediate access        | Long-term data retention and compliance needs        |
| **Cost (Storage)**           | Higher cost per GB                                   | Variable cost, optimized based on access patterns                              | Lower cost than S3 Standard                            | Lower cost than S3 Standard-IA                                  | Lower cost than S3 Standard-IA                             | Lowest cost                                          |
| **Cost (Retrieval)**         | No retrieval cost                                    | Charges apply when moving to IA or Glacier tiers                               | Retrieval costs apply                                  | Retrieval costs apply                                           | Retrieval costs apply                                      | Retrieval costs apply                                |
| **Minimum Storage Duration** | No minimum                                           | 30 days (infrequent tier), 90 days (archive tiers)                             | 30 days                                                | 30 days                                                         | 90 days                                                    | 180 days                                             |

> *Amazon S3 Transfer Acceleration further improves transfer speeds using the AWS global network.*

---

## S3 Pricing Factors

S3 costs are determined by:
1. **Total Data Stored:** Measured in GB.
2. **Storage Class:** Different classes have distinct pricing models.
3. **Data Transfer Out:** Amount of data transferred out of AWS regions.
4. **Number and Type of Requests:** Costs based on operations (GET, PUT, etc.).
5. **Lifecycle Transition Requests:** Fees for moving data between storage classes.

---

## Amazon S3 Policies

An S3 policy typically includes:
- **Action:** Defines allowed or denied operations.
- **Effect:** Indicates whether the action is permitted or denied.
- **Resource:** Specifies the S3 buckets or objects affected.
- **Principal:** Identifies the AWS accounts or users the policy applies to.
- **Sid (Optional):** A unique identifier for the policy statement.
- **Condition (Optional):** Additional restrictions based on specific conditions.

---

## Amazon Relational Database Service (RDS)

RDS is a managed database service supporting engines like MySQL, PostgreSQL, Oracle, SQL Server, and MariaDB. It offers automated backups, scalability, and high availability through multi-AZ deployments, while customers manage data security, schema design, and application-specific configurations.

---

## AWS Database Migration Service (DMS)

AWS DMS simplifies moving databases to AWS or between AWS environments. It supports both homogeneous and heterogeneous migrations with minimal downtime by continuously synchronizing data. Paired with the AWS Schema Conversion Tool, it automatically adapts database schemas across platforms.

---

## AWS Identity and Access Management (IAM)

IAM provides granular control over access to AWS resources:
1. **User:** An individual or application with credentials.
2. **User Group:** A collection of users with common access requirements.
3. **Role:** An identity assumed by trusted entities to gain temporary permissions.
4. **Policies:** JSON documents defining specific permissions.

---

## Root User

The root user is the initial account owner with full administrative control over the AWS account. It should be secured with MFA and used sparingly for high-level tasks only.

---

## AWS Artifact

AWS Artifact offers direct access to AWS security and compliance documentation, such as SOC and PCI reports, supporting regulatory and compliance requirements.

---

## AWS GuardDuty

GuardDuty is an intelligent threat detection service that continuously monitors for malicious behavior using machine learning and anomaly detection, providing real-time alerts for potential security issues.

---

## AWS Shield

AWS Shield provides robust DDoS protection, integrating with CloudFront, ELB, Route 53, and Global Accelerator to defend against network and application layer attacks.

---

## AWS Web Application Firewall (WAF)

AWS WAF allows you to create custom rules to block common web exploits such as SQL injection and cross-site scripting, offering comprehensive Layer 7 protection and real-time metrics.

---

## Security Layers

- **Layer 3 (Network Layer):**  
  Manages packet routing; protected by AWS Shield against volumetric attacks.
- **Layer 4 (Transport Layer):**  
  Handles data transmission protocols; AWS Shield also secures this layer.
- **Layer 7 (Application Layer):**  
  Manages HTTP/HTTPS traffic; AWS WAF provides specialized security.

---

## Customer Compliance Center

The Compliance Center provides answers to compliance questions, risk overviews, and security audit checklists to help ensure cloud deployments meet regulatory standards.

---

## Amazon CloudWatch

CloudWatch collects metrics, logs, and events from AWS resources, enabling automated responses via alarms and providing tools like CloudWatch Logs Insights for deep analysis.

---

## AWS CloudTrail

CloudTrail logs API calls and actions in your AWS account, offering a comprehensive audit trail for security, troubleshooting, and compliance investigations.

---

## AWS Trusted Advisor

Trusted Advisor provides real-time best practice recommendations across cost optimization, performance, security, and fault tolerance, helping you improve your AWS environment.

---

## AWS Billing Dashboard

The Billing Dashboard offers an overview of monthly spending, free tier usage, and cost forecasts, and integrates with Cost Explorer and budgets for expense management.

---

## AWS Consolidated Billing

Consolidated billing unifies multiple AWS accounts under one bill, enabling combined usage discounts and simplifying cost tracking for large organizations.

---

## AWS Budgets

AWS Budgets lets you set custom spending thresholds, monitoring usage and sending alerts when limits are approached or exceeded, ensuring proactive cost control.

---

## AWS Pricing Calculator

The Pricing Calculator estimates AWS service costs based on configuration, providing detailed breakdowns to help plan cloud spending.

---

## AWS Cost and Usage Report (CUR)

CUR aggregates detailed cost data by service, region, or tag, allowing integration with tools like Athena, Redshift, or QuickSight for in-depth analysis.

---

## AWS Cost Explorer

Cost Explorer visualizes historical and forecasted AWS spending, enabling filtering and grouping of cost data to optimize expenditures based on usage trends.

---

## AWS Core Services Overview

| Service                | Description                                  | Use Case                                   | Key Features                                          |
| ---------------------- | -------------------------------------------- | ------------------------------------------ | ----------------------------------------------------- |
| **Amazon EC2**         | Virtual servers in the cloud                 | Compute instances for applications         | Scalability, flexible pricing, various instance types |
| **Amazon S3**          | Scalable object storage service              | File storage and backup                    | Durability, high availability, lifecycle management   |
| **Amazon RDS**         | Managed relational database service          | SQL database hosting                       | Automated backups, scaling, high availability         |
| **Amazon DynamoDB**    | Managed NoSQL database service               | High-performance, low-latency data storage | Fully managed, high throughput, and low latency       |
| **AWS Lambda**         | Serverless compute service                   | Running code in response to events         | No server management, automatic scaling               |
| **Amazon VPC**         | Virtual Private Cloud                        | Isolated network setup                     | Customizable network configuration, security          |
| **Amazon CloudFront**  | Content delivery network (CDN)               | Delivering content with low latency        | Global distribution, edge caching                     |
| **Amazon IAM**         | Identity and Access Management               | User and permission management             | Fine-grained access control, security policies        |
| **Amazon CloudWatch**  | Monitoring and observability service         | Logging, monitoring, and alerts            | Metrics collection, log management, alarms            |
| **AWS CloudFormation** | Infrastructure as Code                       | Automated resource provisioning            | Template-based deployment, version control            |

---

## Support Plans

### Support Plans Comparison

| Feature                             | Basic Support                            | Developer Support              | Business Support                                | Enterprise Support                            |
| ----------------------------------- | ---------------------------------------- | ------------------------------ | ----------------------------------------------- | --------------------------------------------- |
| **Cost**                            | Free                                     | Starts at $29/month            | Starts at $100/month or 3% of monthly AWS usage | Starts at $15,000/month or based on AWS usage |
| **24/7 Access to Customer Support** | No                                       | Yes, via email                 | Yes, via phone, chat, and email                 | Yes, via phone, chat, and email               |
| **Technical Account Manager (TAM)** | No                                       | No                             | No                                              | Yes                                           |
| **AWS Trusted Advisor**             | Core checks                              | Full access to core checks     | Full access                                     | Full access with additional guidance          |
| **Support Response Times**          | None                                     | General guidance: < 24 hours   | Urgent issues: < 1 hour                         | Critical issues: < 15 minutes                 |
| **Third-Party Software Support**    | No                                       | No                             | Yes                                             | Yes                                           |
| **Infrastructure Event Management** | No                                       | No                             | Available for an additional fee                 | Yes                                           |
| **Architecture Support**            | General best practices via documentation | General architectural guidance | Contextual architectural guidance               | Consultative architectural review             |
| **Operations Support**              | No                                       | No                             | Support for common operations                   | Support for complex operations                |
| **Programmatic Case Management**    | No                                       | Yes                            | Yes                                             | Yes                                           |
| **Access to Online Training**       | Limited                                  | Limited                        | Access to selected trainings                    | Full access to AWS training                   |

---

## AWS Marketplace

AWS Marketplace is a digital catalog of thousands of software solutions from independent vendors. It simplifies procurement with flexible pricing options, rapid deployment, and integration with AWS environments.

---

## AWS Cloud Adoption Framework (CAF)

1. **Business Perspective:**  
   Understand how cloud adoption creates value and aligns with business goals through ROI evaluation, risk management, and strategic opportunity identification.

2. **People Perspective:**  
   Align skills and roles with cloud technologies through targeted training and continuous learning.

3. **Governance Perspective:**  
   Establish policies for risk management, cost control, license management, and compliance to integrate IT governance with cloud services.

4. **Platform Perspective:**  
   Design cloud infrastructure that meets business needs by selecting appropriate services and architecting scalable solutions.

5. **Security Perspective:**  
   Implement robust security measures including identity management, data protection, and network security to safeguard assets.

6. **Operations Perspective:**  
   Optimize management of cloud resources with automation, strong incident response, and continuous operational improvements.

---

## 6 Migration Strategies

- **Rehosting (Lift-and-Shift):**  
  Move applications to the cloud with minimal modifications, retaining the existing architecture to minimize disruption.

- **Replatforming:**  
  Make slight adjustments to optimize applications for the cloud, leveraging native capabilities without a complete redesign.

- **Refactoring/Re-architecting:**  
  Redesign applications to be fully cloud-native, using modern best practices and microservices architectures for maximum scalability and resilience.

- **Repurchasing:**  
  Replace legacy applications with cloud-based alternatives (often SaaS), reducing management overhead while enhancing features and reliability.

- **Retaining:**  
  Keep certain legacy applications on-premises if migration is not feasible due to technical, regulatory, or compatibility reasons.

- **Retiring:**  
  Gradually phase out obsolete applications or services to reduce operational complexity and cost.

---

## AWS Snow Family

| Feature              | AWS Snowcone              | AWS Snowball Edge                     | AWS Snowmobile                                                |
| -------------------- | ------------------------- | ------------------------------------- | ------------------------------------------------------------- |
| **Storage Capacity** | Up to 8 TB usable storage | Up to 80 TB usable storage per device | Up to 100 PB per Snowmobile truck                             |
| **Pricing**          | Pay per use (low cost)    | Pay per use (medium cost)             | Pay per use (high cost due to scale and complexity)           |
| **Migration Size**   | Small-scale data transfer | Medium to large-scale data transfer   | Massive-scale data transfer (exabyte-level)                   |

---

## AWS Artificial Intelligence (AI) Services

- **Amazon CodeWhisperer:**  
  Provides real-time code suggestions and security issue identification during development.
- **Amazon Transcribe:**  
  Converts spoken language into text with high accuracy.
- **Amazon Fraud Detector:**  
  Uses machine learning to identify and prevent online fraudulent activities.
- **Amazon Lex:**  
  Builds conversational interfaces for chatbots using voice and text.
- **Amazon Polly:**  
  Converts text into lifelike speech in various languages.
- **Amazon Personalize:**  
  Creates tailored recommendations and dynamic user segmentation using ML.
- **AWS Rekognition:**  
  Analyzes images and videos for object detection and facial recognition.
- **Amazon Comprehend:**  
  Processes natural language to extract sentiment, entities, and key phrases.
- **Amazon Kendra:**  
  Provides enterprise search capabilities powered by machine learning.
- **Amazon SageMaker:**  
  Enables rapid building, training, and deployment of machine learning models.
- **Amazon Translate:**  
  Offers real-time and batch language translation for global applications.

---

## The AWS Well-Architected Framework

### Operational Excellence
Emphasizes automating operations, making reversible changes, continuous process refinement, and proactive failure planning.

### Security
Focuses on robust identity controls, data encryption in transit and at rest, and automating security practices.

### Reliability
Designs systems to quickly recover from failures, scale based on demand, and rigorously test recovery procedures.

### Performance Efficiency
Encourages optimal resource use by selecting the right services, monitoring performance, and experimenting with innovative architectures.

### Cost Optimization
Involves consumption-based models, expenditure monitoring, and eliminating waste through managed services and efficient scaling.

### Sustainability
Considers the environmental, economic, and societal impacts of cloud operations, promoting efficient resource utilization and reduced carbon footprint.

---

## AWS Professional Services

AWS Professional Services offers expert consulting to help design, migrate, and optimize cloud environments. Their tailored guidance covers architecture design, best practices, and modernization strategies.

---

## AWS Concierge and Enterprise Support

- **AWS Concierge Support:**  
  Provides one-on-one technical and strategic guidance for special projects and technology integration.
- **AWS Enterprise Support:**  
  Offers dedicated support with a Technical Account Manager (TAM), 24/7 expert access, and proactive tools like Infrastructure Event Management (IEM).

---

## AWS Config

AWS Config continuously monitors and records resource configurations, tracks changes, and evaluates compliance. It stores historical data and provides visual maps of resource relationships for easier auditing.

---

## AWS CloudEndure

CloudEndure is a disaster recovery solution that replicates applications across clouds or regions. It offers near real-time replication and automatic environment conversion for low RTO and RPO.

---

## AWS Security Hub

Security Hub aggregates and analyzes security findings from multiple AWS services, continuously checking the environment against compliance standards and prioritizing alerts.

---

## AWS Proton

AWS Proton is a managed deployment service for containerized and serverless applications. It streamlines collaboration between development and operations teams through automated deployments and live configuration updates.

---

## AWS Batch

AWS Batch automates planning, scheduling, and execution of batch processing jobs. It scales resources dynamically, integrates with Spot Instances, and automatically retries failed jobs for cost-effective processing.

---

## AWS Systems Manager

A centralized service for managing AWS and on-premises resources.

- **Parameter Store:** Securely stores configuration data and secrets with versioning and encryption.
- **Session Manager:** Provides secure, browser-based or CLI-based access to instances without requiring open ports.
- **Patch Manager:** Automates OS and software patch deployments across instances.

---

## AWS Load Balancers

- **Application Load Balancer (ALB):**  
  Operates at Layer 7 for HTTP/HTTPS traffic with advanced routing and SSL termination.
- **Network Load Balancer (NLB):**  
  Operates at Layer 4 for balancing TCP, UDP, and TLS traffic with ultra-low latency.
- **Classic Load Balancer (CLB):**  
  Legacy option supporting both Layer 4 and 7, primarily used for older applications.
- **Gateway Load Balancer (GWLB):**  
  Operates at Layer 3 to route traffic to virtual appliances, optimized for scaling network functions.

---

## AWS Greengrass

AWS Greengrass extends cloud capabilities to edge devices, enabling local Lambda function execution, data synchronization, and secure communication, even when disconnected from the internet.

---

## Additional Cloud Concepts

- **Servers:**  
  Powerful computers that handle user requests. AWS’s servers are hosted in global data centers and virtualized into smaller units to maximize resource utilization.
- **Usage Types:**  
  - **On Demand:** No long-term commitments or upfront payments.
  - **Pay as you go:** Charges based on actual usage time (hourly or per second).
- **Technical Terms:**  
  - **High Availability:** Systems designed for continuous operation.
  - **Elasticity:** Dynamic resource provisioning based on demand.
  - **Agility:** Increased speed to innovate and deploy.
  - **Durability:** Long-term data protection ensuring integrity.
- **Cloud Computing Models:**  
  - **IaaS:** Infrastructure as a Service (e.g., AWS EC2) provides basic compute, storage, and networking.
  - **PaaS:** Platform as a Service (e.g., AWS Cloud9) offers tools to build and deploy applications.
  - **SaaS:** Software as a Service delivers complete applications managed by the provider.
- **Regions and Availability:**  
  - **Regions:** Physical locations with multiple Availability Zones.
  - **Availability Zones (AZs):** Isolated data centers within regions, connected by low-latency links.
  - **Edge Locations:** Sites used to cache content for faster delivery.
- **AWS Management Console & AWS CLI:**  
  The console offers a web-based interface, while the CLI enables command-line access for automation.

---

## Additional Technology Concepts

- **AWS Backup:**  
  A centralized service that automates backup processes across AWS services with defined backup plans and retention policies.
- **API Gateway:**  
  A fully managed service for creating, publishing, and securing APIs to facilitate system communication.
- **AWS VPN:**  
  Provides secure connectivity between on-premises networks and AWS VPCs over the public internet.
- **DNS & Amazon Route 53:**  
  DNS translates domain names to IP addresses; Route 53 offers domain registration and global DNS routing.
- **AWS Direct Connect:**  
  Provides a dedicated physical connection from on-premises to AWS, improving bandwidth and security.
- **DataSync:**  
  Accelerates large-scale data transfers from on-premises environments to AWS.

- **Additional Compute Services:**  
  - **AWS Fargate:** A serverless compute engine for containers.
  - **AWS Outposts:** Extends AWS infrastructure to on-premises data centers.
  - **AWS Batch:** Processes large-scale batch workloads efficiently.

---

## Additional Developer Tools

- **AWS X-Ray:**  
  Analyzes and debugs distributed applications by providing insights into performance issues and service maps.
- **Amazon SES:**  
  A cloud-based email service for sending marketing, notification, and transactional emails.

---

## Additional Governance and Management Services

- **License Manager:**  
  Tracks and manages software licenses for on-premises and AWS environments, ensuring compliance.
- **Certificate Manager:**  
  Provisions, manages, and deploys SSL/TLS certificates for securing communications.

---

## Additional Billing and Pricing Concepts

- **Free Offer Types:**  
  - **12 Months Free:** Available for new customers for certain services.
  - **Always Free:** Continuous free tier offerings.
  - **Trials:** Short-term free trials for specific services.
- **AWS Price List API:**  
  Provides programmatic access to detailed AWS pricing information.
- **Cost Allocation Tags:**  
  Label AWS resources with key-value pairs for detailed cost tracking and reporting.

---

## AWS Partner Network (APN)

- **Technology Partners:**  
  Offer pre-built software solutions that integrate with AWS.
- **Consulting Partners:**  
  Provide professional services and expertise for AWS deployments.

---

## AWS Organizations

Organizations enable centralized management of multiple AWS accounts with consolidated billing, resource allocation, and Service Control Policies (SCPs) for governance.

---

## AWS Control Tower

Control Tower helps set up and govern a secure, multi-account environment with policy enforcement, centralized management, and a comprehensive dashboard.

---

## AWS Systems Manager

Provides centralized management of AWS resources, enabling automation of operational tasks, resource grouping, and patch management.

---

## Additional Billing and Pricing - Detailed Services

- **EC2 Pricing:**  
  Models include On-Demand, Reserved Instances, Spot Instances, and Savings Plans.
- **Lambda Pricing:**  
  Based on number of requests and execution time, with a free tier of 1 million requests and 400,000 GB-seconds.
- **S3 Pricing:**  
  Determined by storage class, volume, data transfer, and number of requests.
- **RDS Pricing:**  
  Influenced by running hours, database engine, storage, deployment type, and data transfer.

---

## AWS Cost Explorer and Reporting

- **Cost Explorer:**  
  Visualizes historical and forecasted costs.
- **Cost and Usage Reports (CUR):**  
  Provide granular cost data for detailed analysis.
- **Budgets:**  
  Allow custom cost and usage thresholds with alerts.
- **Cost Allocation Tags:**  
  Enable resource tagging for precise cost tracking.

---

## Amazon CloudFront Use Cases

CloudFront is used for caching static assets, streaming live and on-demand video, securing content delivery, running edge functions (Lambda@Edge), and accelerating dynamic content and APIs.

---

## AWS Global Accelerator

Improves application performance by routing traffic through the optimal AWS global network paths and providing static IP addresses for consistent access.

---

## AWS Marketplace

A digital catalog of pre-built software solutions available for purchase, trial, or license, facilitating rapid deployment and integration.

---

## AWS Security and Compliance Services Overview

| Service                                  | Description                                  | Use Case                                         | Key Features                                             |
| ---------------------------------------- | -------------------------------------------- | ------------------------------------------------ | -------------------------------------------------------- |
| **AWS Shield**                           | DDoS protection service                      | Protecting against DDoS attacks                  | Automatic attack mitigation, 24/7 support                |
| **AWS WAF**                              | Web Application Firewall                     | Protecting web applications                      | Customizable rules, integration with CloudFront          |
| **AWS KMS**                              | Key Management Service                       | Managing encryption keys                         | Centralized key management, automatic key rotation       |
| **AWS CloudTrail**                       | API call logging service                     | Monitoring API activity                          | Detailed logs, compliance auditing                       |
| **AWS Config**                           | Resource configuration monitoring            | Compliance tracking and auditing                 | Track configuration changes, automated compliance checks |
| **AWS Macie**                            | Data security and privacy service            | Discover and protect sensitive data              | Automated data classification and protection             |
| **AWS GuardDuty**                        | Threat detection service                     | Continuous security monitoring                   | Threat detection and alerting                            |
| **AWS Inspector**                        | Security assessment service                  | Assessing security vulnerabilities               | Automated security assessments                           |
| **AWS Artifact**                         | Compliance reports and documentation         | Access to compliance reports                     | Access to AWS compliance documentation                   |
| **AWS Cognito**                          | User authentication and access control       | Managing user identities and access              | User pools, identity pools, secure authentication        |
| **AWS Secrets Manager**                  | Manage secrets and sensitive data            | Securely storing and managing secrets            | Automatic rotation, secure access                        |
| **AWS CloudHSM**                         | Hardware security module service             | Managing encryption keys with dedicated hardware | FIPS 140-2 compliance, dedicated HSM devices             |
| **IAM**                                  | Identity and Access Management               | Managing users and permissions                   | Fine-grained access control, security policies           |

---
