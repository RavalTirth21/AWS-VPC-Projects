# 🔒 AWS VPC - AWS NACL (Network Access Control List) Project

## 📘 Project Overview

This project demonstrates how to use **Network ACLs (NACLs)** in AWS to control traffic at the subnet level. The practical covers creating a VPC, subnet, Internet Gateway (IGW), route table, launching an EC2 instance, testing connectivity using ping, and restricting access by denying specific IPs using NACL rules.

---

## 🛠️ AWS Services Used

- **Amazon VPC**
- **Subnets**
- **Internet Gateway (IGW)**
- **Route Tables**
- **EC2 Instance**
- **NACL (Network ACL)**

---

## 🧪 Step-by-Step Implementation

### 1️⃣ VPC Creation

A custom VPC was created to host our resources.

📷 ![VPC Created](./01-VPC-Created.png)

---

### 2️⃣ Subnet Creation

A subnet was created in the custom VPC to launch the EC2 instance.

📷 ![Subnet Created](./02-Subnet-Created.png)

---

### 3️⃣ IGW Created and Attached

An Internet Gateway (IGW) was created and attached to the VPC for internet access.

📷 ![IGW Attached](./03-IGW-Created-&-Attached-with-VPC.png)

---

### 4️⃣ Route Table Configuration

The subnet was associated with a route table that routes `0.0.0.0/0` to the Internet Gateway.

📷 ![Route Table](./04-Route-Table.png)

---

### 5️⃣ EC2 Instance Launch in Configured VPC

An EC2 instance was launched in the configured subnet with SSH and ICMP access.

📷 ![Instance Configured](./05-Instance-with-Configured-VPC.png)

---

### 6️⃣ Security Group Allows SSH and ICMP

The EC2 instance's security group was configured to allow SSH (port 22) and ICMP (ping).

📷 ![SG Allows SSH & ICMP](./06-Instance-with-SSH-ICMP.png)

---

### 7️⃣ PC Can Ping EC2 Instance via Public IP

Ping from the local PC to the EC2 instance public IP is successful.

📷 ![PC Ping Success](./07-PC-Ping-Instance-PublicIP.png)

---

### 8️⃣ Find Public IP of Local Machine

Your public IP address was obtained via [myip.com](https://www.myip.com).

📷 ![My Public IP](./08-My-Public-IP.png)

---

### 9️⃣ NACL Rule Added to Deny Specific IP

A **Deny** rule was added in the NACL to block inbound ICMP traffic from your public IP.

📷 ![Deny IP in NACL](./09-Deny-My-Public-IP.png)

---

### 🔟 Ping Blocked from Your IP

After applying the NACL rule, pinging the EC2 instance from your PC fails.

📷 ![Ping Failed](./10-Failed-to-Ping-Instance-Public-IP.png)

---

## ✅ Final Output

- EC2 instance in a custom VPC.
- Ping and SSH enabled by default.
- NACL successfully blocked ICMP requests from a specific public IP.

---

## 🔐 NACL vs Security Group: Quick Summary

| Feature              | NACL                        | Security Group              |
|----------------------|-----------------------------|-----------------------------|
| Scope                | Subnet Level                | Instance Level              |
| Rule Type            | Stateless (Allow/Deny)      | Stateful (Only Allow)       |
| Traffic Direction    | Inbound and Outbound        | Inbound and Outbound        |
| Rule Processing      | Ordered (Lowest # first)    | All rules evaluated         |

---

## 📂 Folder Structure

AWS-VPC-NACL-Practical/
├── 01-VPC-Created.png
├── 02-Subnet-Created.png
├── 03-IGW-Created-&-Attached-with-VPC.png
├── 04-Route-Table.png
├── 05-Instance-with-Configured-VPC.png
├── 06-Instance-with-SSH-ICMP.png
├── 07-PC-Ping-Instance-PublicIP.png
├── 08-My-Public-IP.png
├── 09-Deny-My-Public-IP.png
├── 10-Failed-to-Ping-Instance-Public-IP.png
└── README.md
