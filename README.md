# 🔐 Secure AWS Cloud Infrastructure with Bastion Host (Production-Ready Architecture)

> A production-style AWS infrastructure demonstrating secure access to private resources using a Bastion Host with complete network isolation.

---

## 📌 Project Overview

This project showcases a **secure and production-ready AWS architecture** where a private EC2 instance is not directly exposed to the internet. Instead, access is strictly controlled through a Bastion Host deployed in a public subnet.

The setup follows **real-world cloud security best practices**, ensuring that sensitive resources remain protected within a private network.

---

## 🏗️ Architecture

User → Bastion Host (Public EC2) → Private EC2 Instance

---

## 🚀 Services Used

- Amazon EC2  
- VPC (Virtual Private Cloud)  
- Public & Private Subnets  
- Internet Gateway  
- Route Tables  
- Security Groups  
- SSH  

---

## 🔧 Implementation Steps

### 1. VPC Configuration
- Created a custom VPC with CIDR block
- Enabled logical network isolation
- Designed subnet segmentation

### 2. Network Setup
- Attached Internet Gateway to VPC
- Configured public and private route tables
- Associated subnets with respective route tables

### 3. EC2 Deployment
- Launched **Bastion Host** in public subnet
- Launched **Private EC2** in private subnet
- Ensured no public IP assigned to private instance

### 4. Security Configuration
- Allowed SSH (port 22) from local machine → Bastion Host
- Allowed SSH from Bastion Host → Private EC2
- Restricted all unnecessary inbound traffic

### 5. Secure Access Flow
- Connected to Bastion Host using SSH
- Accessed Private EC2 via internal network (private IP)
- Verified complete isolation from public internet

---

## 📸 Project Screenshots

### 🌐 VPC & Network Setup

![VPC](images/01-vpc-created.png)
![Subnets](images/02-subnets.png)
![Internet Gateway](images/03-internet-gateway.png)

---

### 🛣️ Routing Configuration

![Route Table](images/04-route-table.png)
![Route Association](images/05-route-table-subnet.png)

---

### 🔐 Security Setup

![Security Group](images/06-security-group.png)
![Security Group Rules](images/13-security-group-rules.png)

---

### 🚀 EC2 Deployment

![EC2 Instance](images/07-ec2-instance.png)
![EC2 Running](images/08-ec2-running.png)
![EC2 Networking](images/09-ec2-networking.png)

---

### 🔗 Secure Access (Bastion Host)

![Bastion Connection](images/10-bastion-connection.png)
![SSH Access](images/11-ec2-ssh.png)

---

### 🧠 Architecture Proof

![VPC Architecture](images/14-vpc-architecture.png)
![Private EC2 No Public IP](images/15-private-no-public-ip.png)

---

### ✅ Final Output

![Web Output](images/12-web-output.png)

---

## 🔐 Key Security Features

- ✅ Private EC2 instance has **no public IP**
- ✅ Access only via Bastion Host (controlled entry point)
- ✅ Network isolation using custom VPC
- ✅ Fine-grained access control using Security Groups
- ✅ Secure SSH communication within private network

---

## 💡 Real-World Relevance

This architecture is widely used in production environments where:
- Sensitive workloads must not be exposed to the internet
- Access needs to be tightly controlled and monitored
- Security and compliance are critical requirements

---

## 📚 Learning Outcomes

- Designed and implemented VPC architecture from scratch  
- Understood subnet isolation and routing mechanisms  
- Gained hands-on experience with secure EC2 access  
- Applied industry-standard cloud security practices  
- Learned Bastion Host-based access control  

---

## 📌 Future Improvements

- Add NAT Gateway for secure outbound internet access  
- Deploy a real-world application on private EC2  
- Integrate CloudWatch monitoring and alerts  
- Implement IAM roles for least-privilege access  

---

## 🏷️ Tags

AWS | EC2 | VPC | Cloud Security | Bastion Host | DevOps | Cloud Architecture  

---

## 👨‍💻 Author

**Ranjan Kumar Upadhyay**
