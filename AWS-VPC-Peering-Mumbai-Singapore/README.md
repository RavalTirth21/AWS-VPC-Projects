# 🌐 AWS VPC Peering Across Regions: Mumbai ↔ Singapore

## 📘 Project Overview

This project demonstrates how to create a **VPC peering connection between two AWS regions**: **Mumbai** and **Singapore**. It involves setting up VPCs, subnets, EC2 instances in each region, configuring route tables, and validating the peering connection through successful ping tests.

---

## 🧰 AWS Services Used

- **Amazon VPC**
- **Subnets**
- **EC2 Instances (Amazon Linux)**
- **VPC Peering**
- **Security Groups**
- **Route Tables**

---

## 🌍 Region Information

- **Mumbai Region (ap-south-1)**  
- **Singapore Region (ap-southeast-1)**

---

## 🔧 Step-by-Step Implementation

### 1️⃣ Create VPC in Mumbai Region

📷 ![01-VPC-Mumbai-Region](./01-VPC-Mumbai-Region.png)

---

### 2️⃣ Create Subnet in Mumbai VPC

📷 ![02-Subnet-Mumbai-Region](./02-Subnet-Mumbai-Region.png)

---

### 3️⃣ Launch EC2 Instance in Mumbai Region

📷 ![03-Instance-Created-with-Mumbai-Region-VPC](./03-Instance-Created-with-Mumbai-Region-VPC.png)

---

### 4️⃣ Create VPC in Singapore Region

📷 ![04-VPC-Singapore-Region](./04-VPC-Singapore-Region.png)

---

### 5️⃣ Create Subnet in Singapore VPC

📷 ![05-Subnet-Singapore-Region](./05-Subnet-Singapore-Region.png)

---

### 6️⃣ Launch EC2 Instance in Singapore Region

📷 ![06-Instance-Created-with-Singapore-Region-VPC](./06-Instance-Created-with-Singapore-Region-VPC.png)

---

### 7️⃣ Create VPC Peering Request from Mumbai

📷 ![07-VPC-Peering-Creating-In-Mumbai-Region](./07-VPC-Peering-Creating-In-Mumbai-Region.png)

---

### 8️⃣ Accept Peering Request in Singapore

📷 ![08-VPC-Peering-Request-Accepted-Singapore-Region](./08-VPC-Peering-Request-Accepted-Singapore-Region.png)

---

### 9️⃣ Modify Mumbai Route Table (Peering + IGW)

📷 ![09-Mumbai-Region-Route-Table-IGW-Peering-Connection-Subnet](./09-Mumbai-Region-Route-Table-IGW-Peering-Connection-Subnet-Association.png)

---

### 🔟 Modify Singapore Route Table (Peering + IGW)

📷 ![10-Singapore-Region-Route-Table-IGW-PeeringConnection-Subnet](./10-Singapore-Region-Route-Table-IGW-PeeringConnection-Subnet-Association.png)

---

### 1️⃣1️⃣ Ping from Mumbai to Singapore (Private IP)

📷 ![11-Ping-From-Mumbai-Region-Instance-to-Singapore-Region-PrivateIP](./11-Ping-From-Mumbai-Region-Instance-to-Singapore-Region-Private-IP.png)

✅ **Success** – Indicates correct peering and route setup.

---

### 1️⃣2️⃣ Ping from Singapore to Mumbai (Private IP)

📷 ![12-Ping-From-Singapore-Region-Instance-to-Mumbai-Region-PrivateIP](./12-Ping-From-Singapore-Region-Instance-to-Mumbai-Region-Private-IP.png)

✅ **Success** – Full bi-directional connectivity verified.

---

## 📁 Folder Structure

AWS-VPC-Peering-Mumbai-Singapore/
├── 01-VPC-Mumbai-Region.png
├── 02-Subnet-Mumbai-Region.png
├── 03-Instance-Created-with-Mumbai-Region-VPC.png
├── 04-VPC-Singapore-Region.png
├── 05-Subnet-Singapore-Region.png
├── 06-Instance-Created-with-Singapore-Region-VPC.png
├── 07-VPC-Peering-Creating-In-Mumbai-Region.png
├── 08-VPC-Peering-Request-Accepted-Singapore-Region.png
├── 09-Mumbai-Region-Route-Table-IGW-Peering-Connection-Subnet-Association.png
├── 10-Singapore-Region-Route-Table-IGW-PeeringConnection-Subnet-Association.png
├── 11-Ping-From-Mumbai-Region-Instance-to-Singapore-Region-Private-IP.png
├── 12-Ping-From-Singapore-Region-Instance-to-Mumbai-Region-Private-IP.png
├── README.md
