# 🔐 Secure AWS Architecture using Bastion Host

## 📌 Project Overview
This project demonstrates a secure AWS architecture where a private EC2 instance is accessed through a Bastion Host (public EC2 instance). The goal is to enhance security by preventing direct access to private resources.

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

## 🔧 Setup Steps

### 1. VPC Configuration
- Created a custom VPC
- Configured public and private subnets

### 2. Network Setup
- Attached Internet Gateway
- Configured route tables and subnet association

### 3. EC2 Instances
- Launched Bastion Host in public subnet
- Launched Private EC2 in private subnet

### 4. Security Configuration
- Allowed SSH (port 22) from local machine to Bastion
- Allowed SSH from Bastion to Private EC2

### 5. Secure Access
- Connected to Bastion Host
- Accessed Private EC2 via Bastion Host

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
![Security Rules](images/13-security-group-rules.png)

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
![Architecture](images/14-vpc-architecture.png)
![Private EC2 No Public IP](images/15-private-no-public-ip.png)

---

### ✅ Final Output
![Web Output](images/12-web-output.png)

---

## 🔐 Key Features
- No direct internet access to private EC2
- Secure SSH access via Bastion Host
- Network isolation using VPC
- Controlled access using Security Groups

---

## 📚 Learning Outcomes
- Understood VPC and subnet design
- Implemented secure architecture using Bastion Host
- Learned EC2 networking and SSH access
- Applied real-world cloud security practices

---

## 📌 Future Improvements
- Add NAT Gateway for outbound internet access
- Deploy application on private EC2
- Integrate CloudWatch monitoring
- Implement IAM roles for better security

---

## 👨‍💻 Author
**Ranjan Kumar Upadhyay**
