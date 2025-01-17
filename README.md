# Lift and Shift Application Workload to AWS

## Description

The project involves migrating a multi-tier web application from a traditional data center to the AWS Cloud using a lift-and-shift strategy. The primary objectives are to modernize the application, reduce operational costs, and enhance scalability by leveraging AWS services and implementing automated deployment processes.

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
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/artifact.png) 
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/instances.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/volumes.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/security%20sgoup.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/target%20groups.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/autoscalling.png)
 ![First try](https://github.com/Vlad774/Lift_and_Shift/blob/main/backend.sh.png)
