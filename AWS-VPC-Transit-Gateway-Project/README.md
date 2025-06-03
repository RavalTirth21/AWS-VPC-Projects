# 🔄 AWS VPC - Transit Gateway 

## 📘 Project Overview

This project demonstrates secure communication between two VPCs (VPC1 and VPC2) using **AWS Transit Gateway (TGW)**. It includes VPC and subnet creation, EC2 instance setup, Transit Gateway attachment, route table configuration, and private IP-based communication across VPCs via SSH and ping.

---

## 🛠️ AWS Services Used

- **Amazon VPC**
- **Subnets**
- **Transit Gateway**
- **Transit Gateway Attachments**
- **Route Tables**
- **EC2 Instances (Private Instances)**
- **Key Pair for SSH**

---

## 🧪 Step-by-Step Implementation

### 1️⃣ Create VPC-1

📷 ![VPC 1](./01-Created-VPC-1.png)

---

### 2️⃣ Create VPC-2

📷 ![VPC 2](./02-Created-VPC-2.png)

---

### 3️⃣ Create Subnet in VPC-1

📷 ![VPC1 Subnet](./03-VPC-1-Subnet.png)

---

### 4️⃣ Create Subnet in VPC-2

📷 ![VPC2 Subnet](./04-VPC-2-Subnet.png)

---

### 5️⃣ Create Transit Gateway

📷 ![Transit Gateway](./05-Created-Transit-Gateway.png)

---

### 6️⃣ Attach VPC1 and VPC2 to Transit Gateway

📷 ![TGW Attachments](./06-TGW-Attachments-VPC1-VPC2-Earlier-Created-VPC.png)

---

### 7️⃣ Launch EC2 Instance in VPC (Earlier Created)

📷 ![Earlier Created Instance](./07-Earlier-Created-VPC-Instance.png)

---

### 8️⃣ Launch EC2 Instance in VPC1

📷 ![VPC1 Instance](./08-VPC1-Instance.png)

---

### 9️⃣ Launch EC2 Instance in VPC2

📷 ![VPC2 Instance](./09-VPC2-Instance.png)

---

### 🔁 Create and Configure Route Tables

#### 🔹 VPC1 Route Table

📷 ![VPC1 Route Table](./10-VPC1-Route-Table.png)

#### 🔹 Associate VPC1 Subnet with Route Table

📷 ![VPC1 Subnet Association](./11-Subnet-Association-VPC-1-Subnet.png)

#### 🔹 VPC2 Route Table

📷 ![VPC2 Route Table](./12-VPC-2-Route-Table.png)

#### 🔹 Associate VPC2 Subnet with Route Table

📷 ![VPC2 Subnet Association](./13-Subnet-Association-VPC-2-Subnet.png)

#### 🔹 Earlier Created VPC Route Table

📷 ![Earlier Created VPC Route Table](./14-Earlier-Created-VPC-Route-Table.png)

#### 🔹 Earlier Created VPC Subnet Association

📷 ![Earlier Created VPC Subnet Association](./15-Earlier-Created-VPC-Subnet-Association.png)

---

### 🔐 SSH into Public Instance

📷 ![SSH Public IP](./16-SSH-with-Earlier-Created-VPC-Instance-Public-IP.png)

---

### 🧪 Ping Using Private IPs

#### 🔹 Ping VPC1 Private IP

📷 ![Ping VPC1](./17-Ping-with-VPC1-Private-IP.png)

#### 🔹 Ping VPC2 Private IP

📷 ![Ping VPC2](./18-Ping-with-VPC2-Private-IP.png)

---

### 🔑 Copy and Configure Private Key

#### 🔹 Copy Key to Public Instance

📷 ![Copy Key](./19-Copy-Private-Key-of-VPC1-VPC2.png)

#### 🔹 Set Key Permissions

📷 ![Key Permission](./20-Permission-To-PrivateKey.png)

---

### 🛜 SSH into Private Instances via Private IPs

#### 🔹 SSH into VPC1 Instance

📷 ![SSH VPC1](./21-SSH-with-VPC1-Private-IP.png)

#### 🔹 SSH into VPC2 Instance

📷 ![SSH VPC2](./22-SSH-with-VPC2-Private-IP.png)

---

## ✅ Final Output

- Successfully connected VPC1 and VPC2 using AWS Transit Gateway.
- Verified private IP-based communication via **ping** and **SSH**.
- Demonstrated secure key copy and permission setup.
- Enabled full private network communication between VPCs across regions/accounts.

---

## 📂 Folder Structure

AWS-VPC-Transit-Gateway-Project/
├── 01-Created-VPC-1.png
├── 02-Created-VPC-2.png
├── 03-VPC-1-Subnet.png
├── 04-VPC-2-Subnet.png
├── 05-Created-Transit-Gateway.png
├── 06-TGW-Attachments-VPC1-VPC2-Earlier-Created-VPC.png
├── 07-Earlier-Created-VPC-Instance.png
├── 08-VPC1-Instance.png
├── 09-VPC2-Instance.png
├── 10-VPC1-Route-Table.png
├── 11-Subnet-Association-VPC-1-Subnet.png
├── 12-VPC-2-Route-Table.png
├── 13-Subnet-Association-VPC-2-Subnet.png
├── 14-Earlier-Created-VPC-Route-Table.png
├── 15-Earlier-Created-VPC-Subnet-Association.png
├── 16-SSH-with-Earlier-Created-VPC-Instance-Public-IP.png
├── 17-Ping-with-VPC1-Private-IP.png
├── 18-Ping-with-VPC2-Private-IP.png
├── 19-Copy-Private-Key-of-VPC1-VPC2.png
├── 20-Permission-To-PrivateKey.png
├── 21-SSH-with-VPC1-Private-IP.png
├── 22-SSH-with-VPC2-Private-IP.png
└── README.md
