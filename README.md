👋 Hi, I’m **Bidyashor**  
🚀 Building my skills in **cloud technologies**, **infrastructure management**, and **automation** through hands-on projects using **AWS**.

# ☁️ CloudInfraOps – Online Examination Server (AWS Project)

### 🎯 Objective
🌱 I’m a fresher exploring **AWS Cloud**, and this project represents my hands-on learning experience.  
I worked on building and deploying a **multi-tier cloud infrastructure** to host an **Online Examination Server**, focusing on designing, securing, and monitoring a scalable environment following **AWS best practices**.

---

## 🧱 Architecture Overview

The solution follows the **CloudInfraOps architecture**, using multiple tiers for scalability, availability, and security.

### **Key Components**
- **VPC:** Custom network with public and private subnets across two Availability Zones.  
- **EC2 (Web Tier):** Auto Scaling group of EC2 instances hosting the examination application.  
- **Application Load Balancer:** Distributes incoming traffic evenly across EC2 instances.  
- **RDS (MySQL):** Managed database deployed in private subnets for secure exam data storage.  
- **ElastiCache (Redis):** Provides caching to improve application performance.  
- **S3 Buckets:**  
  - **S3 Assets Bucket:** Stores static web files and application resources.  
  - **S3 Data Bucket:** Holds exam-related files and user uploads.  
  - **S3 Backup Bucket:** Used for automated RDS snapshots and EBS volume backups.  
  - **S3 CloudTrail Bucket:** Centralized storage for audit and API activity logs.  
- **IAM:** Manages access control and enforces least-privilege permissions.  
- **CloudWatch:** Monitors system metrics and triggers alarms for health events.  
- **SNS:** Sends alert notifications when defined thresholds are breached.  
- **AWS Backup:** Automates data protection for RDS and EC2 volumes.  
- **Systems Manager (SSM):** Enables secure EC2 instance management without SSH.  
- **CloudTrail:** Tracks API activities for auditing and compliance.  

---

## 🏗️ Architecture Diagram
![Architecture Diagram](https://github.com/user-attachments/assets/e393f325-5e99-48c8-806e-c429553b3ce0)

---

## 🔐 Security Design
- Deployed databases and caches in private subnets with no public access.  
- Applied IAM least-privilege roles for each AWS service.  
- Restricted inbound ports using Security Groups and NACLs.  
- Used SSM Session Manager instead of SSH for instance management.  
- Enforced encryption at rest (KMS) and in transit (TLS).  
- Enabled CloudTrail to record all API and account activities.  

---

## 📊 Monitoring & Alerts
- **CloudWatch:** Configured dashboards, metrics, and alarms for EC2, RDS, and ALB.  
- **SNS:** Set up notification topics to send alert emails for resource health issues.  
- **CloudTrail:** Delivered activity logs to S3 for auditing.  
- **AWS Backup:** Managed daily automated backups.  

**Sample Alerts**
- EC2 CPU utilization above 75%  
- Unhealthy ALB targets  
- RDS free storage space below 10%  

---

## 🧠 Key Achievements
- Built a secure and scalable multi-AZ AWS infrastructure from scratch.  
- Automated web-server provisioning with EC2 user data.  
- Implemented fault tolerance using Auto Scaling and Load Balancer.  
- Secured databases and networks using private subnets and IAM policies.  
- Configured monitoring and alerting using CloudWatch and SNS.  
- Automated backup and recovery using AWS Backup.  
- Optimized costs through tagging and resource management.  

---

## 🧩 Technology Stack

| **Layer** | **AWS Services** |
|------------|------------------|
| **Compute** | EC2 (Amazon Linux 2023) |
| **Database** | RDS (MySQL) |
| **Caching** | ElastiCache (Redis) |
| **Storage** | S3 (Assets, Data, Backup, CloudTrail Buckets) |
| **Networking** | VPC, Subnets, NAT Gateway, IGW, Route Tables |
| **Monitoring** | CloudWatch, SNS, CloudTrail |
| **Security** | IAM, Security Groups, KMS, SSM |
| **Automation** | AWS CLI, CloudFormation, User Data |

---

## 🧪 Testing and Validation
1. Accessed the ALB DNS name to confirm the web tier was operational.  
2. Verified EC2 to RDS connectivity through application logs.  
3. Simulated load to test CloudWatch alarms and scaling.  
4. Tested SNS alerts for system performance thresholds.  
5. Validated RDS snapshot restoration and backup recovery.  

---

## 📸 Screenshots
- VPC and subnet configuration  
- ALB and target group health checks  
- Auto Scaling activity  
- RDS database details  
- CloudWatch dashboards and alarms  
- S3 backup and CloudTrail buckets  
- CloudTrail logs  

---

📫 **Connect with Me**
-    🌐 LinkedIn: https://www.linkedin.com/in/bidyashor-cloud
-    📧 Email: bidyashorchingtham12345@gmail.com
-    🐙 GitHub: https://github.com/bidyashor-cloud

---

> **Summary:** This project reflects my learning experience in designing, deploying, and managing a secure, scalable 3-tier AWS infrastructure for an Online Examination Server.
