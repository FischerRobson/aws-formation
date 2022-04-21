# AWS Certificate

> Important Links:
> 

[AWS glossary](https://docs.aws.amazon.com/general/latest/gr/glos-chap.html)

[Princípios básicos da AWS - Visão geral](https://aws.amazon.com/pt/getting-started/fundamentals-overview/)

[O que é cloud computing (computação em nuvem)? - Amazon Web Services](https://aws.amazon.com/pt/what-is-cloud-computing/)

[Tipos de cloud computing - Amazon Web Services](https://aws.amazon.com/pt/types-of-cloud-computing/)

[O que é AWS? Como funciona Amazon Web Services](https://aws.amazon.com/pt/what-is-aws/)

[Cloudcraft - Draw AWS diagrams](https://app.cloudcraft.co/)

AWS service offerings: 

- Compute
- Storage
- Network Security
- Blockchain
- Machine Learning
- Artificial Inteligence
- Robot Development

**Pay for What you Need**: Principle of pay-as-you-go pricing model, you only pay for what you use!

Client-Server Model:

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled.png)

In computing, a **client** can be a web browser or desktop application that a person interacts with to make requests to computer servers. A **server** can be services such as Amazon Elastic Compute Cloud (Amazon EC2), a type of virtual server.

For example, suppose that a client makes a request for a news article, the score in an online game, or a funny video. The server evaluates the details of this request and fulfills it by returning the information to the client.

# Cloud

The on-demand delivery of IT resources over the internet with pay-as-you-go pricing.

So, AWS has the resources you need, when you need then, flexibility in so many IT products.

The Undifferentiated heavy lifting of IT: tasks that are common, often repetitive, these are the tasks that AWS help you.

When selecting a cloud strategy, a company must consider factors such as required cloud application components, preferred resource management tools, and any legacy IT infrastructure requirements.

### Cloud-Based Deployment

- Run all parts of the application in the cloud.
- Migrate existing applications to the cloud.
- Design and build new applications in the cloud.

In a **cloud-based deployment** model, you can migrate existing applications to the cloud, or you can design and build new applications in the cloud. You can build those applications on low-level infrastructure that requires your IT staff to manage them. Alternatively, you can build them using higher-level services that reduce the management, architecting, and scaling requirements of the core infrastructure.

For example, a company might create an application consisting of virtual servers, databases, and networking components that are fully based in the cloud.

### On-Premises Deployment

- Deploy resources by using virtualization and resource management tools.
- Increase resource utilization by using application management and virtualization technologies.

**On-premises deployment** is also known as a *private cloud* deployment. In this model, resources are deployed on premises by using virtualization and resource management tools.

For example, you might have applications that run on technology that is fully kept in your on-premises data center. Though this model is much like legacy IT infrastructure, its incorporation of application management and virtualization technologies helps to increase resource utilization.

### Hybrid Deployment

- Connect cloud-based resources to on-premises infrastructure.
- Integrate cloud-based resources with legacy IT applications.

In a **hybrid deployment**, cloud-based resources are connected to on-premises infrastructure. You might want to use this approach in a number of situations. For example, you have legacy applications that are better maintained on premises, or government regulations require your business to keep certain records on premises.

For example, suppose that a company wants to use cloud services that can automate batch data processing and analytics. However, the company has several legacy applications that are more suitable on premises and will not be migrated to the cloud. With a hybrid deployment, the company would be able to keep the legacy applications on premises while benefiting from the data and analytics services that run in the cloud.

### Benefits of Cloud Computing:

- **Trade upfront expense for variable expense**
- **Stop spending money to run and maintain data centers**
- **Stop guessing capacity**
- **Benefit from massive economies of scale**
- **Increase speed and agility**
- **Go global in minutes**

# Amazon Elastic Compute Cloud (EC2):

Virtual Server.

Highly flexible, cost-effective and quick.

Multitenancy: sharing underlying hardware between virtual machines.

Chose the OS, the softwares, databases → complete control.

Resizible → Vertical Scaling (Memory and CPU).

Network control → private/public, request control.

Compute as a Server (CaaS).

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%201.png)

### Each EC2 instance type is grouped under an instance family.

The different instance families are:

- General purpouse → balanced resources of compute, memory and network resources, used in Web Server or code repositories.
- Compute optimized → ideal for intense compute tasks, like gaming servers, high performance computing, scientific modeling.
- Memory optimized →  ideal for intense memory tasks. Designed to deliver fast performance for workloads that process large datasets in memory. Are more ideal for workloads that process large datasets in memory, such as high-performance databases.
- Accelerated computing → floating point number calculations, graphics processing, data pattern matching, utilize hardware acclerators.
- Storage optimized → high performance for locally stored data. Are designed for workloads that require high, sequential read and write access to large datasets on local storage. The question does not specify the size of data that will be processed.

### Pricing

- On-Demand → The instances run continuously until you stop them, and you pay for only the compute time you use.
- Savings Plans → enable you to reduce your compute costs by committing to a consistent amount of compute usage for a 1-year or 3-year term.
- Reserved Instances → are a billing discount applied to the use of On-Demand Instances in your account. You can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term, and Scheduled Reserved Instances for a 1-year term. You realize greater cost savings with the 3-year option.
- Spot Instances → ideal for workloads with flexible start and end times, or that can withstand interruptions.
- Dedicated Hosts → are physical servers with Amazon EC2 instance capacity that is fully dedicated to your use.

### ****Scalability****

involves beginning with only the resources you need and designing your architecture to automatically respond to changing demand by scaling out or in. As a result, you pay for only the resources you use. You don’t have to worry about a lack of computing capacity to meet your customers’ needs.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%202.png)

- *Dynamic scaling* responds to changing demand.
- *Predictive scaling* automatically schedules the right number of Amazon EC2 instances based on predicted demand.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%203.png)

### Load Balancer

Is an application that takes in request and routes them to te instanteces to be processed.

Properly distribute traffic with high performance, cost-efficient, highly avaliable, automatically scalable

# Elastic Load Balancing (ELB)

is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances.

Decoupled Architecture.

Regional construct, a single URL

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%204.png)

### **Messaging and queuing**

Tightly Decoupled Architecture (breaks if one instance fails) → Loosely Coupled Achitecture (single fails wont cause cascading failure).

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%205.png)

# Amazon Simple Queue Service (SQS)

Send, store and recive messages between software components at any volume.

The data coitained within a message is called payload. The messages are send into a queue.

# Amazon Simple Notification Service (SNS)

SNS Topic: Channel for messages to be delivered, configure subscribers, that recive that message.

AWS Lambda Functions, HTTPS/HTTP web hooks.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%206.png)

# Serverless / AWS Lambda

You cannot see or access the underlying infrastructure. With serverless computing, you can focus more on innovating new products and features instead of maintaining servers.

Host short running functions, service-oriented applications, event driven applications, no provisioning or managing servers.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%207.png)

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%208.png)

# ****Amazon Elastic Container Service (Amazon ECS)****

is a highly scalable, high-performance container management system that enables you to run and scale containerized applications on AWS.

# ****Amazon Elastic Kubernetes Service (Amazon EKS)****

****is a fully managed service that you can use to run Kubernetes on AWS.

# ****AWS Fargate****

is a serverless compute engine for containers. It works with both Amazon ECS and Amazon EKS. When using AWS Fargate, you do not need to provision or manage servers. AWS Fargate manages your server infrastructure for you. You can focus more on innovating and developing your applications, and you pay only for the resources that are required to run your containers.

# AWS Global Infrastructure

The infrastructure is divided into regions, each isolated from the others, the information is only made available to the others if it is explicitly informed. They are connect via Fiber Netwok managed by AWS. Are geographically isolated, and contain Availability Zones.

To select a Region, consider:

- **Compliance**: Depending on your company and location, you might need to run your data out of specific areas. For example, if your company requires all of its data to reside within the boundaries of the UK, you would choose the London Region.
- **Proximity**: Selecting a Region that is close to your customers will help you to get content to them faster.
- **Available Services**: Sometimes, the closest Region might not have all the features that you want to offer to customers. AWS is frequently innovating by creating new services and expanding on features within existing services.
- **Pricing**: Suppose that you are considering running applications in both the United States and Brazil. The way Brazil’s tax structure is set up, it might cost 50% more to run the same workload out of the São Paulo Region compared to the Oregon Region.

The Availability Zone is one or more Data Centers, with redundant power, networking and connectivity. Run across at least in two AZs in a Region. Availability Zones are located tens of miles apart from each other.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%209.png)

# Amazon CloundFront (its a CDN)

Is a service that helps deliver data, video, APIs, applications around the world with low latency, using Edge Locations.

**Edge Locations** are out of Regions, run too a DNS, kown as Amazon Route 53. An edge location ****is a site that Amazon CloudFront uses to store cached copies of your content closer to your customers for faster delivery.

AWS Outposts are mini regions installed in your data center, owned and operated by AWS.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2010.png)

Everything in AWS is an API call.

You can use AWS Management Console, AWS CLI, AWS SDKs.

Console: Test environments, view AWS bills, view monitoring, work with non-technical resources.

CLI: make API call in the terminal, write an run scripts.

SDKs: interact with AWS resources through various programming languages.

# AWS Elastic Beanstalk

Is a service that helps you provision EC2-based environments. Dont need to provision and manage all of these pieces separately. Focus on business application, not infrastructure.

With **AWS Elastic Beanstalk**, you provide code and configuration settings, and Elastic Beanstalk deploys the resources necessary to perform the following tasks:

- Adjust capacity
- Load balancing
- Automatic scaling
- Application health monitoring

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2011.png)

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2012.png)

# AWS CloudFormation

Infrastructure as code tool used to define a wirde variety of AWS resources in a declarative way using JSON or YAML. Suports Storage, Database, Analytics, Machine Learning.

AWS CloudFormation provisions your resources in a safe, repeatable manner, enabling you to frequently build your infrastructure and applications without having to perform manual actions. It determines the right operations to perform when managing your stack and rolls back changes automatically if it detects errors.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2013.png)

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2014.png)

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2015.png)

# Amazon Virtual Private Cloud (Amazon VPC)

A VPC lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. These resources can be public facing so they have access to the internet, or private with no internet access, usually for backend services like databases or application servers. The public and private grouping of resources are known as subnets and they are ranges of IP addresses in your VPC.

Amazon VPC enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. Within a virtual private cloud (VPC), you can organize your resources into subnets. A **subnet** is a section of a VPC that can contain resources such as Amazon EC2 instances.

When a customer requests data from an application hosted in the AWS Cloud, this request is sent as a packet. A **packet** is a unit of data sent over the internet or a network.

### **Internet gateway**

To allow public traffic from the internet to access your VPC, you attach an **internet gateway** to the VPC.

![Captura de Tela 2022-04-13 às 12.29.19.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-13_as_12.29.19.png)

### **Virtual private gateway**

To access private resources in a VPC, you can use a **virtual private gateway**.

Here’s an example of how a virtual private gateway works. You can think of the internet as the road between your home and the coffee shop. Suppose that you are traveling on this road with a bodyguard to protect you. You are still using the same road as other customers, but with an extra layer of protection.

The bodyguard is like a virtual private network (VPN) connection that encrypts (or protects) your internet traffic from all the other requests around it.

![Captura de Tela 2022-04-13 às 12.30.34.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-13_as_12.30.34.png)

# AWS Direct Connect

Is a service that enables you to establish a dedicated private connection between your data center and a VPC. The private connection that AWS Direct Connect provides helps you to reduce network costs and increase the amount of bandwidth that can travel through your network.

![Captura de Tela 2022-04-13 às 12.31.31.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-13_as_12.31.31.png)

# Network Access Control List

A network access control list (ACL) is a virtual firewall that controls inbound and outbound traffic at the subnet level.

Each AWS account includes a default network ACL. When configuring your VPC, you can use your account’s default network ACL or create custom network ACLs.

By default, your account’s default network ACL **allows all inbound and outbound traffic**, but you can modify it by adding your own rules. For custom network ACLs, all inbound and outbound traffic is denied until you add rules to specify which traffic to allow. Additionally, all network ACLs have an explicit deny rule. This rule ensures that if a packet doesn’t match any of the other rules on the list, the packet is denied.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2016.png)

# Security Groups

A security group is a virtual firewall that controls inbound and outbound traffic for an Amazon EC2 instance. By default, a security group **denies all inbound traffic and allows all outbound traffic**. You can add custom rules to configure which traffic to allow or deny.

If you have multiple Amazon EC2 instances within a subnet, you can associate them with the same security group or use different security groups for each instance.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2017.png)

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2018.png)

## ****Subnets****

**Public subnets** contain resources that need to be accessible by the public, such as an online store’s website.

**Private subnets** contain resources that should be accessible only through your private network, such as a database that contains customers’ personal information and order histories.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2019.png)

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2020.png)

# Domain Name System

DNS resolution involves a customer DNS resolver communicating with a company DNS server.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2021.png)

# ****Amazon Route 53****

is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS.

Amazon Route 53 connects user requests to infrastructure running in AWS (such as Amazon EC2 instances and load balancers). It can route users to infrastructure outside of AWS.

Another feature of Route 53 is the ability to manage the DNS records for domain names. You can register new domain names directly in Route 53. You can also transfer DNS records for existing domain names managed by other domain registrars. This enables you to manage all of your domain names within a single location.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2022.png)

# Instance Storage

Default store for EC2 instance. Block-level storage volumes behave like physical hard drives. An **[instance store](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html)** provides temporary block-level storage for an Amazon EC2 instance. An instance store is disk storage that is physically attached to the host computer for an EC2 instance, and therefore has the same lifespan as the instance. When the instance is terminated, you lose any data in the instance store.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2023.png)

# Amazon Elastic Block Store (EBS)

is a service that provides block-level storage volumes that you can use with Amazon EC2 instances. If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available. 

To create an EBS volume, you define the configuration (such as volume size and type) and provision it. After you create an EBS volume, it can attach to an Amazon EC2 instance.

Because EBS volumes are for data that needs to persist, it’s important to back up the data. You can take incremental backups of EBS volumes by creating Amazon EBS snapshots.

Its stored within a single AZ.

![Captura de Tela 2022-04-18 às 16.58.07.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-18_as_16.58.07.png)

### Snapshoting

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2024.png)

An **[EBS snapshot](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html)** is an incremental backup. This means that the first backup taken of a volume copies all the data. For subsequent backups, only the blocks of data that have changed since the most recent snapshot are saved.

Incremental backups are different from full backups, in which all the data in a storage volume copies each time a backup occurs. The full backup includes data that has not changed since the most recent backup.

# Amazon Simple Storage Service (S3)

is a service that provides object-level storage. Amazon S3 stores data as objects in buckets.

You can upload any type of file to Amazon S3, such as images, videos, text files, and so on. For example, you might use Amazon S3 to store backup files, media files for a website, or archived documents. Amazon S3 offers unlimited storage space. The maximum file size for an object in Amazon S3 is 5 TB.

When you upload a file to Amazon S3, you can set permissions to control visibility and access to it. You can also use the Amazon S3 versioning feature to track changes to your objects over time.

![Captura de Tela 2022-04-18 às 16.46.08.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-18_as_16.46.08.png)

- Standart
    - Designed for frequently accessed data
    - Stores data in a minimum of three Availability Zones
    
    S3 Standard provides high availability for objects. This makes it a good choice for a wide range of use cases, such as websites, content distribution, and data analytics. S3 Standard has a higher cost than other storage classes intended for infrequently accessed data and archival storage.
    
- Standart-Infrequent
    - Ideal for infrequently accessed data
    - Similar to S3 Standard but has a lower storage price and higher retrieval price
    
    S3 Standard-IA is ideal for data infrequently accessed but requires high availability when needed. Both S3 Standard and S3 Standard-IA store data in a minimum of three Availability Zones. S3 Standard-IA provides the same level of availability as S3 Standard but with a lower storage price and a higher retrieval price.
    
- Glacier
    - Low-cost storage designed for data archiving
    - Able to retrieve objects within a few minutes to hours
    
    S3 Glacier is a low-cost storage class that is ideal for data archiving. For example, you might use this storage class to store archived customer records or older photos and video files.
    

![Captura de Tela 2022-04-18 às 16.58.56.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-18_as_16.58.56.png)

### Object (S3) or Block(EBS) Storage?

Object storage treats any file as a complete, discreet object. Now this is great for documents, and images, and video files that get uploaded and consumed as entire objects, but every time there's a change to the object, you must re-upload the entire file. There are no delta updates. Block storage breaks those files down to small component parts or blocks. This means, for that 80-gigabyte file, when you make an edit to one scene in the film and save that change, the engine only updates the blocks where those bits live. If you're making a bunch of micro edits, using EBS, elastic block storage, is the perfect use case. If you were using S3, every time you saved the changes, the system would have to upload all 80 gigabytes, the whole thing, every time.

# Amazon Elastic File System (EFS)

is a scalable file system used with AWS Cloud services and on-premises resources. As you add and remove files, Amazon EFS grows and shrinks automatically. It can scale on demand to petabytes without disrupting applications.

In **file storage**, multiple clients (such as users, applications, servers, and so on) can access data that is stored in shared file folders. In this approach, a storage server uses block storage with a local file system to organize files. Clients access data through file paths.

Compared to block storage and object storage, file storage is ideal for use cases in which a large number of services and resources need to access the same data at the same time.

Its stored across multiple AZs.

# **Amazon Relational Database Service (Amazon RDS)**

![Captura de Tela 2022-04-19 às 11.42.08.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-19_as_11.42.08.png)

In a **relational database**, data is stored in a way that relates it to other pieces of data.

An example of a relational database might be the coffee shop’s inventory management system. Each record in the database would include data for a single item, such as product name, size, price, and so on.

Relational databases use **structured query language (SQL)** to store and query data. This approach allows data to be stored in an easily understandable, consistent, and scalable way. For example, the coffee shop owners can write a SQL query to identify all the customers whose most frequently purchased drink is a medium latte.

is a service that enables you to run relational databases in the AWS Cloud.

Amazon RDS is a managed service that automates tasks such as hardware provisioning, database setup, patching, and backups. With these capabilities, you can spend less time completing administrative tasks and more time using data to innovate your applications. You can integrate Amazon RDS with other services to fulfill your business and operational needs, such as using AWS Lambda to query your database from a serverless application.

Amazon RDS provides a number of different security options. Many Amazon RDS database engines offer encryption at rest (protecting data while it is stored) and encryption in transit (protecting data while it is being sent and received).

Supported database engines include:

- Amazon Aurora
- PostgreSQL
- MySQL
- MariaDB
- Oracle Database
- Microsoft SQL Server

# ****Amazon Aurora****

is an enterprise-class relational database. It is compatible with MySQL and PostgreSQL relational databases. It is up to five times faster than standard MySQL databases and up to three times faster than standard PostgreSQL databases.

Amazon Aurora helps to reduce your database costs by reducing unnecessary input/output (I/O) operations, while ensuring that your database resources remain reliable and available.

Consider Amazon Aurora if your workloads require high availability. It replicates six copies of your data across three Availability Zones and continuously backs up your data to Amazon S3.

# Amazon DynamoDB

![Captura de Tela 2022-04-19 às 11.42.55.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-19_as_11.42.55.png)

is a non-relational, NoSQL database. It is purpose built. Meaning it has specific use cases, and it isn't the best fit for every workload out there. It has millisecond response time. It's fully managed, and it's highly scalable. Its serverless, which means that you do not have to provision, patch, or manage servers. You also do not have to install, maintain, or operate software.

is a key-value database service. It delivers single-digit millisecond performance at any scale.

As the size of your database shrinks or grows, DynamoDB automatically scales to adjust for changes in capacity while maintaining consistent performance.

# ****Amazon Redshift****

is a data warehousing service that you can use for big data analytics. It offers the ability to collect data from many sources and helps you to understand relationships and trends across your data.

Data warehouses are engineered specifically for this kind of big data, where you are looking at historical analytics as opposed to operational analysis.

# ****AWS Database Migration Service (AWS DMS)****

enables you to migrate relational databases, nonrelational databases, and other types of data stores.

With AWS DMS, you move data between a source database and a target database. [The source and target databases](https://aws.amazon.com/dms/resources) can be of the same type or different types. During the migration, your source database remains operational, reducing downtime for any applications that rely on the database.

For example, suppose that you have a MySQL database that is stored on premises in an Amazon EC2 instance or in Amazon RDS, its a Homogeneous migration. Consider the MySQL database to be your source database. Using AWS DMS, you could migrate your data to a target database, such as an Amazon Aurora database.

Heterogeneous migrations is s a two-step process. Since the schema structures, data types, and database code are different between source and target, we first need to convert them using the AWS Schema Conversion Tool. This will convert the source schema and code to match that of the target database. The next step is then to use DMS to migrate data from the source database to the target database.

**Development and test database migrations:** Enabling developers to test applications against production data without affecting production users.

**Database consolidation:** Combining several databases into a single database.

**Continuous replication:** Sending ongoing copies of your data to other target sources instead of doing a one-time migration.

# **Amazon DocumentDB**

is a document database service that supports MongoDB workloads. (MongoDB is a document database program.)

# **Amazon Neptune**

is a graph database service.

You can use Amazon Neptune to build and run applications that work with highly connected datasets, such as recommendation engines, fraud detection, and knowledge graphs.

# **Amazon Quantum Ledger Database (Amazon QLDB)**

is a ledger database service.

You can use Amazon QLDB to review a complete history of all the changes that have been made to your application data.

# **Amazon Managed Blockchain**

is a service that you can use to create and manage blockchain networks with open-source frameworks.

Blockchain is a distributed ledger system that lets multiple parties run transactions and share data without a central authority.

# **Amazon ElastiCache**

is a service that adds caching layers on top of your databases to help improve the read times of common requests.

It supports two types of data stores: Redis and Memcached.

# **Amazon DynamoDB Accelerator**

is an in-memory cache for DynamoDB.

It helps improve response times from single-digit milliseconds to microseconds.

# Security

![Captura de Tela 2022-04-19 às 13.58.34.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-19_as_13.58.34.png)

![Captura de Tela 2022-04-19 às 14.09.28.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-19_as_14.09.28.png)

The shared responsibility model divides into customer responsibilities (commonly referred to as “security in the cloud”) and AWS responsibilities (commonly referred to as “security of the cloud”).

- Customers
    
    Customers are responsible for the security of everything that they create and put *in* the AWS Cloud.
    
    When using AWS services, you, the customer, maintain complete control over your content. You are responsible for managing security requirements for your content, including which content you choose to store on AWS, which AWS services you use, and who has access to that content. You also control how access rights are granted, managed, and revoked.
    
    The security steps that you take will depend on factors such as the services that you use, the complexity of your systems, and your company’s specific operational and security needs. Steps include selecting, configuring, and patching the operating systems that will run on Amazon EC2 instances, configuring security groups, and managing user accounts.
    
- AWS
    
    AWS is responsible for security *of* the cloud.
    
    AWS operates, manages, and controls the components at all layers of infrastructure. This includes areas such as the host operating system, the virtualization layer, and even the physical security of the data centers from which services operate.
    
    AWS is responsible for protecting the global infrastructure that runs all of the services offered in the AWS Cloud. This infrastructure includes AWS Regions, Availability Zones, and edge locations.
    
    AWS manages the security of the cloud, specifically the physical infrastructure that hosts your resources, which include:
    
    - Physical security of data centers
    - Hardware and software infrastructure
    - Network infrastructure
    - Virtualization infrastructure
    
    Although you cannot visit AWS data centers to see this protection firsthand, AWS provides several reports from third-party auditors. These auditors have verified its compliance with a variety of computer security standards and regulations.
    

# ****AWS Identity and Access Management (IAM)****

Authentication and Authorization as a Service.

Enables you to manage access to AWS services and resources securely.

IAM gives you the flexibility to configure access based on your company’s specific operational and security needs.

### Root User

When you first create an AWS account, you begin with an identity known as the **[root user](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html)**.

The root user is accessed by signing in with the email address and password that you used to create your AWS account. You can think of the root user as being similar to the owner of the coffee shop. It has complete access to all the AWS services and resources in the account.

![Captura de Tela 2022-04-19 às 14.32.50.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-19_as_14.32.50.png)

### IAM Users

An **IAM user** is an identity that you create in AWS. It represents the person or application that interacts with AWS services and resources. It consists of a name and credentials.

By default, when you create a new IAM user in AWS, it has no permissions associated with it. To allow the IAM user to perform specific actions in AWS, such as launching an Amazon EC2 instance or creating an Amazon S3 bucket, you must grant the IAM user the necessary permissions.

*We recommend that you create individual IAM users for each person who needs to access AWS. Even if you have multiple employees who require the same level of access, you should create individual IAM users for each of them.*

### IAM Polices

An **IAM policy** is a document that allows or denies permissions to AWS services and resources.

IAM policies enable you to customize users’ levels of access to resources. For example, you can allow users to access all of the Amazon S3 buckets within your AWS account, or only a specific bucket.

*Follow the security principle of **least privilege** when granting permissions. By following this principle, you help to prevent users or roles from having more permissions than needed to perform their tasks.*

```json
{
	"version": 2012-07-11,
	"Statement": {
		"Effect": "Allow",
		"Action": ["s3:ListObject", "s3:GetObject"],
		"Resource": [
			"arn:aws:s3::: awsdoc-example-bucket/", 
			"arn:aws:s3::: awsdoc-example-bucket/*"
		]
	}
}
```

*In this example, the IAM policy is allowing specific actions within Amazon S3: ListObject and GetObject. The policy also mentions a specific bucket ID: awsdoc-example-bucket.*

### IAM Groups

An IAM group is a collection of IAM users. When you assign an IAM policy to a group, all users in the group are granted permissions specified by the policy.

![Captura de Tela 2022-04-19 às 14.46.24.png](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Captura_de_Tela_2022-04-19_as_14.46.24.png)

### IAM Roles

An IAM role is an identity that you can assume to gain temporary access to permissions.

Before an IAM user, application, or service can assume an IAM role, they must be granted permissions to switch to the role. When someone assumes an IAM role, they abandon all previous permissions that they had under a previous role and assume the permissions of the new role.

*IAM roles are ideal for situations in which access to services or resources needs to be granted temporarily, instead of long-term.*

In IAM, multi-factor authentication (MFA) provides an extra layer of security for your AWS account.

## AWS Organizations

Suppose that your company has multiple AWS accounts. You can use **[AWS Organizations](https://aws.amazon.com/organizations)** to consolidate and manage multiple AWS accounts within a central location.

When you create an organization, AWS Organizations automatically creates a **root**, which is the parent container for all the accounts in your organization.

In AWS Organizations, you can centrally control permissions for the accounts in your organization by using **[service control policies (SCPs)](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html)**. SCPs enable you to place restrictions on the AWS services, resources, and individual API actions that users and roles in each account can access.

Advantages is centralized management of all your AWS accounts, this means you can use the primary account of your organization to consolidate and pay for all member accounts. Another advantage of consolidated billing is bulk discounts, implement hierarchical groupings of your accounts to meet security, compliance, or budgetary needs, control over the AWS services and API actions that each account can access as an administrator of the primary account of an organization.

In AWS Organizations, you can group accounts into **organizational units** (OUs) to make it easier to manage accounts with similar business or security requirements. When you apply a policy to an OU, all the accounts in the OU automatically inherit the permissions specified in the policy.

# AWS Artifact

Depending on your company’s industry, you may need to uphold specific standards. An audit or inspection will ensure that the company has met those standards.

**[AWS Artifact](https://aws.amazon.com/artifact)** is a service that provides on-demand access to AWS security and compliance reports and select online agreements. AWS Artifact consists of two main sections: AWS Artifact Agreements and AWS Artifact Reports.

**Agreements**: In AWS Artifact Agreements, you can review, accept, and manage agreements for an individual account and for all your accounts in AWS Organizations. Different types of agreements are offered to address the needs of customers who are subject to specific regulations, such as the Health Insurance Portability and Accountability Act (HIPAA).

**Reports**: AWS Artifact Reports provide compliance reports from third-party auditors. These auditors have tested and verified that AWS is compliant with a variety of global, regional, and industry-specific security standards and regulations. AWS Artifact Reports remains up to date with the latest reports released. You can provide the AWS audit artifacts to your auditors or regulators as evidence of AWS security controls.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2025.png)

### ****Customer Compliance Center****

Contains resources to help you learn more about AWS compliance.

In the Customer Compliance Center, you can read customer compliance stories to discover how companies in regulated industries have solved various compliance, governance, and audit challenges.

Additionally, the Customer Compliance Center includes an auditor learning path. This learning path is designed for individuals in auditing, compliance, and legal roles who want to learn more about how their internal operations can demonstrate compliance using the AWS Cloud.

## ****Denial-of-service attacks****

A **denial-of-service (DoS) attack** is a deliberate attempt to make a website or application unavailable to users.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2026.png)

For example, an attacker might flood a website or application with excessive network traffic until the targeted website or application becomes overloaded and is no longer able to respond. If the website or application becomes unavailable, this denies service to users who are trying to make legitimate requests.

## ****Distributed denial-of-service attacks****

In a distributed denial-of-service (DDoS) attack, multiple sources are used to start an attack that aims to make a website or application unavailable. This can come from a group of attackers, or even a single attacker. The single attacker can use multiple infected computers (also known as “bots”) to send excessive traffic to a website or application.

To help minimize the effect of DoS and DDoS attacks on your applications, you can use **[AWS Shield](https://aws.amazon.com/shield)**.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2027.png)

# AWS Shield

**AWS Shield Standard** automatically protects all AWS customers at no cost. It protects your AWS resources from the most common, frequently occurring types of DDoS attacks.

As network traffic comes into your applications, AWS Shield Standard uses a variety of analysis techniques to detect malicious traffic in real time and automatically mitigates it.

**AWS Shield Advanced** is a paid service that provides detailed attack diagnostics and the ability to detect and mitigate sophisticated DDoS attacks.

It also integrates with other services such as Amazon CloudFront, Amazon Route 53, and Elastic Load Balancing. Additionally, you can integrate AWS Shield with AWS WAF by writing custom rules to mitigate complex DDoS attacks.

# ****AWS Key Management Service (AWS KMS)****

enables you to perform encryption operations through the use of **cryptographic keys**. A cryptographic key is a random string of digits used for locking (encrypting) and unlocking (decrypting) data. You can use AWS KMS to create, manage, and use cryptographic keys. You can also control the use of keys across a wide range of services and in your applications.

With AWS KMS, you can choose the specific levels of access control that you need for your keys. For example, you can specify which IAM users and roles are able to manage keys. Alternatively, you can temporarily disable keys so that they are no longer in use by anyone. Your keys never leave AWS KMS, and you are always in control of them.

# ****AWS WAF****

Is a web application firewall that lets you monitor network requests that come into your web applications.

AWS WAF works together with Amazon CloudFront and an Application Load Balancer. Recall the network access control lists that you learned about in an earlier module. AWS WAF works in a similar way to block or allow traffic. However, it does this by using a **[web access control list (ACL)](https://docs.aws.amazon.com/waf/latest/developerguide/web-acl.html)** to protect your AWS resources.

# ****Amazon Inspector****

helps to improve the security and compliance of applications by running automated security assessments. It checks applications for security vulnerabilities and deviations from security best practices, such as open access to Amazon EC2 instances and installations of vulnerable software versions.

After Amazon Inspector has performed an assessment, it provides you with a list of security findings. The list prioritizes by severity level, including a detailed description of each security issue and a recommendation for how to fix it. However, AWS does not guarantee that following the provided recommendations resolves every potential security issue. Under the shared responsibility model, customers are responsible for the security of their applications, processes, and tools that run on AWS services.

# ****Amazon GuardDuty****

is a service that provides intelligent threat detection for your AWS infrastructure and resources. It identifies threats by continuously monitoring the network activity and account behavior within your AWS environment.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2028.png)

After you have enabled GuardDuty for your AWS account, GuardDuty begins monitoring your network and account activity. You do not have to deploy or manage any additional security software. GuardDuty then continuously analyzes data from multiple AWS sources, including VPC Flow Logs and DNS logs.

If GuardDuty detects any threats, you can review detailed findings about them from the AWS Management Console. Findings include recommended steps for remediation. You can also configure AWS Lambda functions to take remediation steps automatically in response to GuardDuty’s security findings.

# ****Amazon CloudWatch****

is a web service that enables you to monitor and manage various metrics and configure alarm actions based on data from those metrics.

CloudWatch uses **[metrics](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/working_with_metrics.html)** to represent the data points for your resources. AWS services send metrics to CloudWatch. CloudWatch then uses these metrics to create graphs automatically that show how performance has changed over time.

### Alarms

With CloudWatch, you can create **[alarms](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/AlarmThatSendsEmail.html)** that automatically perform actions if the value of your metric has gone above or below a predefined threshold.

For example, suppose that your company’s developers use Amazon EC2 instances for application development or testing purposes. If the developers occasionally forget to stop the instances, the instances will continue to run and incur charges.

In this scenario, you could create a CloudWatch alarm that automatically stops an Amazon EC2 instance when the CPU utilization percentage has remained below a certain threshold for a specified period. When configuring the alarm, you can specify to receive a notification whenever this alarm is triggered.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2029.png)

The CloudWatch **[dashboard](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Dashboards.html)** feature enables you to access all the metrics for your resources from a single location. For example, you can use a CloudWatch dashboard to monitor the CPU utilization of an Amazon EC2 instance, the total number of requests made to an Amazon S3 bucket, and more. You can even customize separate dashboards for different business purposes, applications, or resources.

# ****AWS CloudTrail****

Records API calls for your account. The recorded information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more. You can think of CloudTrail as a “trail” of breadcrumbs (or a log of actions) that someone has left behind them.

Recall that you can use API calls to provision, manage, and configure your AWS resources. With CloudTrail, you can view a complete history of user activity and API calls for your applications and resources.

Events are typically updated in CloudTrail within 15 minutes after an API call. You can filter events by specifying the time and date that an API call occurred, the user who requested the action, the type of resource that was involved in the API call, and more.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2030.png)

### ****CloudTrail Insights****

Within CloudTrail, you can also enable **[CloudTrail Insights](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-insights-events-with-cloudtrail.html)**. This optional feature allows CloudTrail to automatically detect unusual API activities in your AWS account.

# ****AWS Trusted Advisor****

is a web service that inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices.

Trusted Advisor compares its findings to AWS best practices in five categories**: cost optimization, performance, security, fault tolerance, and service limits**. For the checks in each category, Trusted Advisor offers a list of recommended actions and additional resources to learn more about AWS best practices.

The guidance provided by AWS Trusted Advisor can benefit your company at all stages of deployment. For example, you can use AWS Trusted Advisor to assist you while you are creating new workflows and developing new applications. Or you can use it while you are making ongoing improvements to existing applications and resources.

![Untitled](AWS%20Certificate%20a39333b005b844609951d3105d58ea38/Untitled%2031.png)