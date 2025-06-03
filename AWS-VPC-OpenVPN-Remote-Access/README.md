# 🔐 AWS-VPC-OpenVPN Setup for Remote Access

## 📘 Project Overview

This project demonstrates how to set up a secure OpenVPN server on AWS within a VPC using a Windows EC2 instance. 

---

## 🧰 AWS Services Used

- **Amazon VPC**
- **Public Subnet**
- **Windows EC2 Instance**
- **OpenVPN Access Server**
- **PuTTY & Key Generator**
- **PuTTY Configuration**
- **OpenVPN Client (Mobile/Desktop)**

---

## 🔧 Step-by-Step Implementation

### 1️⃣ Create Public & Private Subnets

📷 ![01-Public-Private-Subnet-Creation](./01-Public-Private-Subnet-Creation.png)

---

### 2️⃣ Configure Route Table for VPC

📷 ![02-Route-Table-of-Created-VPC](./02-Route-Table-of-Created-VPC.png)

---

### 3️⃣ Launch Windows EC2 Instance

📷 ![03-Windows-Instance-Created](./03-Windows-Instance-Created.png)

---

### 4️⃣ Decrypt the Password for Windows EC2

📷 ![04-Windows-Instance-Decrypted-Password](./04-Windows-Instance-Decrypted-Password.png)

---

### 5️⃣ Launch OpenVPN AMI

📷 ![05-AMI-For-OpenVPN](./05-AMI-For-OpenVPN.png)

---

### 6️⃣ OpenVPN Instance Created

📷 ![06-OpenVPN-Instance-Created](./06-OpenVPN-Instance-Created.png)

---

### 7️⃣ Generate `.ppk` Key Using PuTTYgen

📷 ![07-Creating-.ppk-Key-For-OpenVPN](./07-Creating-.ppk-Key-For-OpenVPN.png)

---

### 8️⃣ `.ppk` Key File Created

📷 ![08-.ppk-Key-Created](./08-.ppk-Key-Created.png)

---

### 9️⃣ Configure PuTTY to Use the Public IP

📷 ![09-Public-IP-OpenVPN-Instance-Putty-Configuration](./09-Public-IP-OpenVPN-Instance-Putty-Configuration.png)

---

### 🔟 Set Path to `.ppk` Key in PuTTY

📷 ![10-Path-to-.ppk-Key-Putty-Configuration](./10-Path-to-.ppk-Key-Putty-Configuration.png)

---

### 1️⃣1️⃣ Accept PuTTY Security Alert

📷 ![11-Putty-Security-Alert-Accept](./11-Putty-Security-Alert-Accept.png)

---

### 1️⃣2️⃣ Log in with OpenVPN Default User

📷 ![12-Give-Password-OpenVPN-Account](./12-Give-Password-OpenVPN-Account.png)

---

### 1️⃣3️⃣ OpenVPN URL Generated

📷 ![13-Generated-URL](./13-Generated-URL.png)

---

### 1️⃣4️⃣ Access URL in OpenVPN Client

📷 ![14-Put-URL-in-OpenVPN-Connect](./14-Put-URL-in-OpenVPN-Connect.png)

---

### 1️⃣5️⃣ Import Username & Password into Client

📷 ![15-Username-Password-Import](./15-Username-Password-Import.png)

---

### 1️⃣6️⃣ VPN Connected Successfully

📷 ![16-Connected](./16-Connected.png)

---

### 1️⃣7️⃣ Remote Desktop: Enter Computer & Username

📷 ![17-Remote-Desktop-Connection-Computer-Username-Connect](./17-Remote-Desktop-Connection-Computer-Username-Connect.png)

---

### 1️⃣8️⃣ Give Decrypted Password 

📷 ![18-Give-Decrypt-Windows-Password](./18-Give-Decrypt-Windows-Password.png)

---

### 1️⃣9️⃣ Successfully Connected to Windows Instance via VPN

📷 ![19-Connected-To-Windows-Instance](./19-Connected-To-Windows-Instance.png)

---

### 2️⃣0️⃣ Disconnected VPN than Windows Instance Remote Connection Disconnected

📷 ![20-OpenVPN-Disconnected-Windows-Server-Disconnected](./20-OpenVPN-Disconnected-Windows-Server-Disconnected.png)

---

## ✅ Outcome

- OpenVPN Access Server successfully deployed on AWS.
- Connected securely using OpenVPN Connect client.
- Remotely accessed Windows EC2 instance over VPN.

---

## 📁 Folder Structure

AWS-VPC-OpenVPN-Remote-Access/
├── 01-Public-Private-Subnet-Creation.png
├── 02-Route-Table-of-Created-VPC.png
├── 03-Windows-Instance-Created.png
├── 04-Windows-Instance-Decrypted-Password.png
├── 05-AMI-For-OpenVPN.png
├── 06-OpenVPN-Instance-Created.png
├── 07-Creating-.ppk-Key-For-OpenVPN.png
├── 08-.ppk-Key-Created.png
├── 09-Public-IP-OpenVPN-Instance-Putty-Configuration.png
├── 10-Path-to-.ppk-Key-Putty-Configuration.png
├── 11-Putty-Security-Alert-Accept.png
├── 12-Give-Password-OpenVPN-Account.png
├── 13-Generated-URL.png
├── 14-Put-URL-in-OpenVPN-Connect.png
├── 15-Username-Password-Import.png
├── 16-Connected.png
├── 17-Remote-Desktop-Connection-Computer-Username-Connect.png
├── 18-Give-Decrypt-Windows-Password.png
├── 19-Connected-To-Windows-Instance.png
├── 20-OpenVPN-Disconnected-Windows-Server-Disconnected.png
├── README.md
