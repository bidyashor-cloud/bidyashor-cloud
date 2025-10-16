👋 Hi, I’m **Bidyashor**  

🚀 Building skills in **AWS Cloud**, **SysOps**, **cloud administration**, and **automation** through hands-on projects.

# ☁️ CloudInfraOps – Online Examination Server (AWS Project)

### 🎯 Objective
I designed and deployed a **multi-tier cloud infrastructure** on **AWS** to host an **Online Examination Server**.  
This project demonstrates my ability to build, secure, monitor, and manage scalable AWS environments following SysOps and Cloud Engineer best practices.

---

## 🧱 Architecture Overview

The solution follows the **CloudInfraOps architecture**, using multiple tiers for scalability, availability, and security.

### **Key Components**
- **VPC:** Custom network with public and private subnets across two Availability Zones.  
- **EC2 (Web Tier):** Auto Scaling group of EC2 instances hosting the examination application.  
- **Application Load Balancer:** Distributes incoming traffic evenly across EC2 instances.  
- **RDS (MySQL):** Managed database deployed in private subnets for secure exam data storage.  
- **ElastiCache (Redis):** Provides caching to improve application performance.  
- **S3 Bucket:** Stores backups, logs, and static assets.  
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

## ⚙️ Deployment Phases


- **Phase 1. Networking:** Build a custom VPC with public and private subnets across two AZs. 
- **Phase 2. IAM & Security:** Create IAM roles, policies, and enable CloudTrail for access control and auditing. 
- **Phase 3. Security Groups:** Configure inbound and outbound rules for ALB, EC2, RDS, and Redis. 
- **Phase 4. EC2 Setup:** Launch EC2 instances in an Auto Scaling Group using a Launch Template with user-data scripts. 
- **Phase 5. Load Balancer:** Deploy an Application Load Balancer for traffic routing and distribution. 
- **Phase 6. Database Layer:** Provision an RDS MySQL database with automatic backups. 
- **Phase 7. Caching Layer:** Integrate ElastiCache Redis for session and data caching. 
- **Phase 8. Monitoring:** Enable CloudWatch metrics, alarms, and SNS notifications. 
- **Phase 9. Backup & Storage:** Configure S3 and AWS Backup for logs and data protection. 
- **Phase 10. Automation:** Automate deployments with AWS CLI and CloudFormation templates. 

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


 **CloudWatch:** Configured dashboards, metrics, and alarms for EC2, RDS, and ALB. 
 **SNS:** Set up notification topics to send alert emails for resource health issues. 
 **CloudTrail:** Delivered activity logs to S3 for auditing. 
 **AWS Backup:** Managed daily automated backups. 

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

Layers & AWS Service
------------------------------------------
- **Compute:**  EC2 (Amazon Linux ) 
- **Database:**  RDS (MySQL) 
- **Caching:**  ElastiCache (Redis) 
- **Storage:**  S3 
- **Networking:**  VPC, Subnets, NAT, IGW, Route Tables 
- **Monitoring:**  CloudWatch, SNS, CloudTrail 
- **Security:**  IAM, Security Groups, KMS, SSM 
- **Automation:**  AWS CLI, CloudFormation, User Data 

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
- S3 backup bucket  
- CloudTrail logs  

---
📫 Connect with Me
-    🌐 LinkedIn: https://www.linkedin.com/in/bidyashor-cloud
-    📧 Email: bidyashorchingtham12345@gmail.com
-    🐙 GitHub: https://github.com/bidyashor-cloud

---

> **Summary:** Designed and deployed a secure, scalable 3-tier AWS infrastructure for an Online Examination Server, demonstrating real-world SysOps and Cloud Engineering practices.

