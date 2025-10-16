👋 Hi, I’m **Bidyashor**  
🚀 Building my skills in **cloud technologies**, **infrastructure management**, and **automation** through hands-on projects using **AWS**.

# ☁️ CloudInfraOps – Online Examination Server (AWS Project)

### 🎯 Objective
🌱 I’m a fresher exploring **AWS Cloud**, and this project represents my hands-on learning experience.  
I worked on building and deploying a **multi-tier cloud infrastructure** to host an **Online Examination Server**, focusing on designing, securing, and monitoring a scalable environment following **AWS best practices**.

---

## 🧱 Architecture Overview

This project follows a **3-tier CloudInfraOps architecture** designed for scalability, availability, and security.

### **Key Components**
- **VPC:** Custom network with public, private, and database subnets across two Availability Zones.  
- **EC2 (Web Tier):** Auto Scaling Group of web servers hosting the application.  
- **Application Load Balancer:** Distributes traffic evenly across EC2 instances.  
- **RDS (MySQL):** Managed database for secure exam data storage (Multi-AZ).  
- **ElastiCache (Redis):** Caching layer for faster performance and session management.  
- **S3 Buckets:** Used for static assets, backups, and CloudTrail logs.  
- **IAM:** Access control and least-privilege permissions across AWS services.  
- **CloudWatch & SNS:** Monitoring, metrics, and alert notifications.  
- **AWS Backup:** Automated daily backups for RDS and EC2 volumes.  
- **Systems Manager (SSM):** Secure EC2 access and automation without SSH.  
- **CloudTrail:** Centralized API activity logging for auditing and compliance.  

---

## 🏗️ Architecture Diagram
![Architecture Diagram](https://github.com/user-attachments/assets/e393f325-5e99-48c8-806e-c429553b3ce0)

---

## 🔐 Security Design
- Private subnets for RDS and ElastiCache (no public access).  
- IAM roles with least-privilege permissions.  
- Restricted inbound ports using Security Groups and NACLs.  
- Managed access via **SSM Session Manager** (no SSH keys).  
- Encryption at rest (KMS) and in transit (TLS).  
- CloudTrail enabled for account-level auditing.  

---

## 📊 Monitoring & Alerts
- **CloudWatch:** Dashboards, metrics, and alarms for EC2, RDS, and ALB.  
- **SNS:** Email alerts for key resource health events.  
- **CloudTrail:** Logs all API actions to S3 for auditing.  
- **AWS Backup:** Automated recovery and data protection.  

**Example Alerts**
- EC2 CPU utilization above 75%  
- Unhealthy ALB targets  
- RDS free storage space below 10%  

---

## 🧠 Key Highlights
- Built a **secure, scalable, and highly available** AWS infrastructure.  
- Implemented **Auto Scaling** and **Load Balancer** for fault tolerance.  
- Used **RDS** and **ElastiCache** in private subnets for better security.  
- Configured **monitoring and alerts** via CloudWatch and SNS.  
- Automated **backups and recovery** using AWS Backup.  
- Followed **AWS Well-Architected Framework** principles.  

---

## 🧩 Technology Stack

| **Layer** | **AWS Services** |
|------------|------------------|
| **Compute** | EC2 (Amazon Linux 2, Auto Scaling) |
| **Database** | RDS (MySQL) |
| **Caching** | ElastiCache (Redis) |
| **Storage** | S3 (Assets, Backups, Logs) |
| **Networking** | VPC, Subnets, NAT Gateway, IGW, Route Tables |
| **Monitoring** | CloudWatch, SNS, CloudTrail |
| **Security** | IAM, Security Groups, KMS, SSM |
| **Automation** | AWS CLI, CloudFormation, User Data, AWS Backup |

---

## 🧪 Validation Steps
1. Verified ALB DNS endpoint to ensure web tier functionality.  
2. Tested EC2-to-RDS connectivity through app logs.  
3. Simulated load to validate CloudWatch alarms and scaling.  
4. Tested SNS email alerts for high CPU and health check failures.  
5. Validated RDS snapshot restoration and backup recovery.  

---

## 📸 Screenshots
- VPC and subnet setup  
- ALB and target group health checks  
- Auto Scaling activity  
- RDS instance configuration  
- CloudWatch dashboards and alarms  
- S3 backup and CloudTrail logs  

---

📫 **Connect with Me**
- 🌐 [LinkedIn](https://www.linkedin.com/in/bidyashor-cloud)  
- 📧 **bidyashorchingtham12345@gmail.com**  
- 🐙 [GitHub](https://github.com/bidyashor-cloud)

---

> **Summary:** Built and deployed a secure, scalable 3-tier AWS architecture for an Online Examination Server, demonstrating practical cloud design, deployment, and monitoring skills.
