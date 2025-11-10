<a id="readme-top"></a>

<h3 align="center">Cloud Applications (D782)</h3>

  <p align="center">
    Course D782 – CloudCampusIQ: Cloud Architecture, Security, and Cost Management  
    <br /><br />
    <a href="https://d3ldni9a03nobl.cloudfront.net/">View Deployed Application</a>
</div>

## About the Project

This project was completed for **D782 – Cloud Applications**, which focuses on designing, deploying, and securing scalable cloud-based solutions.
The project implements **CloudCampusIQ**, a cloud-hosted learning management platform that supports **10,000 concurrent users**, leveraging Amazon Web Services (AWS) for scalability, performance, and compliance.

The implementation demonstrates architecture design, deployment automation, IAM security controls, cost optimization, and monitoring—all aligned with industry best practices for secure, reliable, and cost-effective cloud operations.

## Course Information

**Course:** D782 – Cloud Applications
**Focus:** Building and managing scalable, secure cloud solutions through AWS.

### Competencies

**Cloud Architecture Design**
The graduate designs cloud-based solutions that support scalability, security, and performance needs for enterprise-scale workloads.

**Cloud Deployment and Configuration**
The graduate deploys and configures applications in a cloud environment using managed service models to simplify scalability and maintenance.

**Security and Monitoring**
The graduate applies security, monitoring, and cost management controls to ensure the confidentiality, integrity, and availability of cloud-hosted applications.

## Task 1 – Cloud Architecture & Storage

Task 1 focuses on the **architecture and infrastructure design** of CloudCampusIQ, detailing the use of AWS managed services to ensure performance, security, and cost control.

### Key Highlights

* **Architecture Overview**

  * Application deployed within a secure **AWS VPC** using **Elastic Beanstalk (PaaS)**.
  * **Amazon S3** stores course materials (videos, PDFs, lab files).
  * **AWS CloudFront** distributes content globally with low latency.
  * **AWS IAM** enforces role-based access and compliance with **FERPA**, **GDPR**, and **SOC 2**.

* **Cloud Service Model**

  * Selected **Platform as a Service (PaaS)** via Elastic Beanstalk for simplified management, scalability, and cost predictability.

* **Storage and Lifecycle Management**

  * S3 lifecycle rules transition files to Glacier after 30 days and delete unused assets after 1 year, reducing long-term storage costs.
  * Integrated with IAM for access control and CloudFront for efficient global content delivery.

## Task 2 – Cloud Security, Monitoring, and Cost Management

Task 2 focuses on deploying, securing, and monitoring the AWS environment supporting CloudCampusIQ.

### Key Highlights

* **Security Configuration**

  * Implemented **IAM roles** with **least privilege** to isolate permissions.
  * Enabled **HTTPS** using **AWS Certificate Manager**.
  * Restricted inbound network traffic to **port 443 only** via **Security Groups**.
  * Configured **CloudWatch Logs** for access monitoring and auditing.

* **Deployment and Hosting**

  * Deployed sample application on **AWS Elastic Beanstalk**, which automates provisioning, load balancing, and scaling.
  * Verified deployment through the public endpoint:
    [https://d3ldni9a03nobl.cloudfront.net/](https://d3ldni9a03nobl.cloudfront.net/)

* **Monitoring and Cost Controls**

  * Set up **CloudWatch alarms** to trigger alerts when CPU utilization > 70% for 5 minutes.
  * Created **AWS Cost Explorer dashboard** to track service-level costs for Elastic Beanstalk, S3, and CloudFront.
  * Ensures reliable performance while staying within a projected **$25K/month operating budget**.

* **Benefits Summary**

  * Strong security posture with IAM, HTTPS, and network isolation.
  * Fully automated scaling and load balancing through Elastic Beanstalk.
  * Cost transparency and budget adherence via Cost Explorer.
  * Global availability and performance through CloudFront.

## Architecture Overview

**Core Services Used:**

* AWS Elastic Beanstalk (PaaS)
* Amazon S3 (storage + lifecycle management)
* Amazon CloudFront (CDN)
* AWS IAM (identity and access)
* Amazon CloudWatch (monitoring and logging)
* AWS Cost Explorer (budget tracking)

This architecture supports up to 10,000 concurrent learners and provides fault-tolerant, auto-scaled, secure access to educational content across regions.

## References

Amazon Web Services Inc. (2025). *AWS Documentation*.
AWS. (2025). *Elastic Beanstalk, S3, CloudFront, and CloudWatch Best Practices*.

## Contact

**Silver Alcid**
[Website](https://silveralcid.com) • [Outlook](mailto:silveralcid@outlook.com)
