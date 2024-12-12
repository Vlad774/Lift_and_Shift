# Lift and Shift Application Workload to AWS

## Description

This project migrates the vProfile multi-tier web application stack from a traditional data center to AWS Cloud using a lift-and-shift strategy. The goal is to modernize the application, reduce costs, and enhance scalability through AWS services and automated deployment.

##Technologies

- **Backend:** Spring MVC, Spring Security, Spring Data JPA.
- **Build/Deploy:** Maven, Tomcat.
- **Frontend:** JSP.
- **Database:** MySQL.
- **Cache/Messaging:** Memcached, RabbitMQ.
- **Search:** ElasticSearch.

## Key AWS Services

- **Compute & Networking:** EC2, Elastic Load Balancer (ELB), Auto Scaling.
- **Storage:** Amazon S3, EBS.
- **DNS & Security:** Route 53, IAM, ACM.
- **Automation:** Infrastructure as Code (IaC) via scripts.

## Architecture Overview

- Users access the application through GoDaddy DNS, routed to an HTTPS-secured ELB.
- Tomcat Instances handle backend services, scaling dynamically with Auto Scaling.
- MySQL, Memcached, RabbitMQ, and ElasticSearch operate as backend components, accessed via private DNS zones.
- Artifacts are built with Maven, stored in S3, and deployed to instances via IaC.
  

## Walk-through:


 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/Diagramm.png) 
 ![First try](https://github.com/Vlad774/IoT-WebOps-Stack-with-IaC/blob/main/VM_machine_Setup_IAC.png) 
 ![First try](https://github.com/Vlad774/IoT-WebOps-Stack-with-IaC/blob/main/Automated_setup.png)
 ![First try](https://github.com/Vlad774/IoT-WebOps-Stack-with-IaC/blob/main/config.png)
