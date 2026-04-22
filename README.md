# 🔐 Secure AWS Architecture using Bastion Host

## 📌 Project Overview

This project demonstrates a secure AWS architecture where a private EC2 instance is accessed through a bastion host (public EC2 instance). The goal is to enhance security by preventing direct access to private resources.

---

## 🏗️ Architecture

```
User → Bastion Host (Public EC2) → Private EC2 Instance
```

---

## 🚀 Services Used

* Amazon EC2
* VPC (Virtual Private Cloud)
* Subnets (Public & Private)
* Security Groups
* SSH

---

## 🔧 Setup Steps

### 1. VPC Configuration

* Created a custom VPC
* Configured public and private subnets

### 2. EC2 Instances

* Launched a **Bastion Host** in public subnet
* Launched a **Private EC2** in private subnet

### 3. Security Configuration

* Allowed SSH (port 22) from local machine to Bastion
* Allowed SSH from Bastion to Private EC2

### 4. SSH Access

* Connected to Bastion Host from local machine
* Accessed Private EC2 via Bastion

---

## 📸 Screenshots

### Bastion Connection

![Bastion](screenshots/bastion-connection.png)

### Private EC2 Access

![Private EC2](screenshots/private-ec2-ssh.png)

---

## 🔐 Key Features

* No direct internet access to private EC2
* Secure SSH access via Bastion Host
* Network isolation using VPC

---

## 📚 Learning Outcomes

* Understood VPC and subnet design
* Implemented secure access using Bastion Host
* Gained hands-on experience with EC2 and SSH

---

## 📌 Future Improvements

* Implement NAT Gateway for internet access
* Deploy a web server on private EC2
* Add monitoring using CloudWatch

---

## 👨‍💻 Author

Ranjan Kumar Upadhyay
