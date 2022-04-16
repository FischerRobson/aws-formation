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
- Artifical Inteligence
- Robot Development

**Pay for What you Need**: Principle of pay-as-you-go pricing model, you only pay for what you use!

Client-Server Model:

![Untitled](AWS%20Certif%20a3933/Untitled.png)

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

![Untitled](AWS%20Certif%20a3933/Untitled%201.png)

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

![Untitled](AWS%20Certif%20a3933/Untitled%202.png)

- *Dynamic scaling* responds to changing demand.
- *Predictive scaling* automatically schedules the right number of Amazon EC2 instances based on predicted demand.

![Untitled](AWS%20Certif%20a3933/Untitled%203.png)

### Load Balancer

Is an application that takes in request and routes them to te instanteces to be processed.

Properly distribute traffic with high performance, cost-efficient, highly avaliable, automatically scalable

# Elastic Load Balancing (ELB)

is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances.

Decoupled Architecture.

Regional construct, a single URL

![Untitled](AWS%20Certif%20a3933/Untitled%204.png)

### **Messaging and queuing**

Tightly Decoupled Architecture (breaks if one instance fails) → Loosely Coupled Achitecture (single fails wont cause cascading failure).

![Untitled](AWS%20Certif%20a3933/Untitled%205.png)

# Amazon Simple Queue Service (SQS)

Send, store and recive messages between software components at any volume.

The data coitained within a message is called payload. The messages are send into a queue.

# Amazon Simple Notification Service (SNS)

SNS Topic: Channel for messages to be delivered, configure subscribers, that recive that message.

AWS Lambda Functions, HTTPS/HTTP web hooks.

![Untitled](AWS%20Certif%20a3933/Untitled%206.png)

# Serverless / AWS Lambda

You cannot see or access the underlying infrastructure. With serverless computing, you can focus more on innovating new products and features instead of maintaining servers.

Host short running functions, service-oriented applications, event driven applications, no provisioning or managing servers.

![Untitled](AWS%20Certif%20a3933/Untitled%207.png)

![Untitled](AWS%20Certif%20a3933/Untitled%208.png)

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

![Untitled](AWS%20Certif%20a3933/Untitled%209.png)

# Amazon CloundFront (its a CDN)

Is a service that helps deliver data, video, APIs, applications around the world with low latency, using Edge Locations.

**Edge Locations** are out of Regions, run too a DNS, kown as Amazon Route 53. An edge location ****is a site that Amazon CloudFront uses to store cached copies of your content closer to your customers for faster delivery.

AWS Outposts are mini regions installed in your data center, owned and operated by AWS.

![Untitled](AWS%20Certif%20a3933/Untitled%2010.png)

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

![Untitled](AWS%20Certif%20a3933/Untitled%2011.png)

![Untitled](AWS%20Certif%20a3933/Untitled%2012.png)

# AWS CloudFormation

Infrastructure as code tool used to define a wirde variety of AWS resources in a declarative way using JSON or YAML. Suports Storage, Database, Analytics, Machine Learning.

AWS CloudFormation provisions your resources in a safe, repeatable manner, enabling you to frequently build your infrastructure and applications without having to perform manual actions. It determines the right operations to perform when managing your stack and rolls back changes automatically if it detects errors.

![Untitled](AWS%20Certif%20a3933/Untitled%2013.png)

![Untitled](AWS%20Certif%20a3933/Untitled%2014.png)

![Untitled](AWS%20Certif%20a3933/Untitled%2015.png)

# Amazon Virtual Private Cloud (Amazon VPC)

A VPC lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. These resources can be public facing so they have access to the internet, or private with no internet access, usually for backend services like databases or application servers. The public and private grouping of resources are known as subnets and they are ranges of IP addresses in your VPC.

Amazon VPC enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. Within a virtual private cloud (VPC), you can organize your resources into subnets. A **subnet** is a section of a VPC that can contain resources such as Amazon EC2 instances.

When a customer requests data from an application hosted in the AWS Cloud, this request is sent as a packet. A **packet** is a unit of data sent over the internet or a network.

### **Internet gateway**

To allow public traffic from the internet to access your VPC, you attach an **internet gateway** to the VPC.

![Captura de Tela 2022-04-13 às 12.29.19.png](AWS%20Certif%20a3933/Captura_de_Tela_2022-04-13_as_12.29.19.png)

### **Virtual private gateway**

To access private resources in a VPC, you can use a **virtual private gateway**.

Here’s an example of how a virtual private gateway works. You can think of the internet as the road between your home and the coffee shop. Suppose that you are traveling on this road with a bodyguard to protect you. You are still using the same road as other customers, but with an extra layer of protection.

The bodyguard is like a virtual private network (VPN) connection that encrypts (or protects) your internet traffic from all the other requests around it.

![Captura de Tela 2022-04-13 às 12.30.34.png](AWS%20Certif%20a3933/Captura_de_Tela_2022-04-13_as_12.30.34.png)

# AWS Direct Connect

Is a service that enables you to establish a dedicated private connection between your data center and a VPC. The private connection that AWS Direct Connect provides helps you to reduce network costs and increase the amount of bandwidth that can travel through your network.

![Captura de Tela 2022-04-13 às 12.31.31.png](AWS%20Certif%20a3933/Captura_de_Tela_2022-04-13_as_12.31.31.png)

# Network Access Control List

A network access control list (ACL) is a virtual firewall that controls inbound and outbound traffic at the subnet level.

Each AWS account includes a default network ACL. When configuring your VPC, you can use your account’s default network ACL or create custom network ACLs.

By default, your account’s default network ACL **allows all inbound and outbound traffic**, but you can modify it by adding your own rules. For custom network ACLs, all inbound and outbound traffic is denied until you add rules to specify which traffic to allow. Additionally, all network ACLs have an explicit deny rule. This rule ensures that if a packet doesn’t match any of the other rules on the list, the packet is denied.

![Untitled](AWS%20Certif%20a3933/Untitled%2016.png)

# Security Groups

A security group is a virtual firewall that controls inbound and outbound traffic for an Amazon EC2 instance. By default, a security group **denies all inbound traffic and allows all outbound traffic**. You can add custom rules to configure which traffic to allow or deny.

If you have multiple Amazon EC2 instances within a subnet, you can associate them with the same security group or use different security groups for each instance.

![Untitled](AWS%20Certif%20a3933/Untitled%2017.png)

![Untitled](AWS%20Certif%20a3933/Untitled%2018.png)

## ****Subnets****

**Public subnets** contain resources that need to be accessible by the public, such as an online store’s website.

**Private subnets** contain resources that should be accessible only through your private network, such as a database that contains customers’ personal information and order histories.

![Untitled](AWS%20Certif%20a3933/Untitled%2019.png)

![Untitled](AWS%20Certif%20a3933/Untitled%2020.png)

# Domain Name System

DNS resolution involves a customer DNS resolver communicating with a company DNS server.

![Untitled](AWS%20Certif%20a3933/Untitled%2021.png)

# ****Amazon Route 53****

is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS.

Amazon Route 53 connects user requests to infrastructure running in AWS (such as Amazon EC2 instances and load balancers). It can route users to infrastructure outside of AWS.

Another feature of Route 53 is the ability to manage the DNS records for domain names. You can register new domain names directly in Route 53. You can also transfer DNS records for existing domain names managed by other domain registrars. This enables you to manage all of your domain names within a single location.

![Untitled](AWS%20Certif%20a3933/Untitled%2022.png)