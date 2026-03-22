# aws-ec2-ssh
# AWS EC2 Hands-On

## 📌 Overview

This project demonstrates launching and connecting to an AWS EC2 instance using both browser-based access and SSH via Bash.

---

## 🚀 Steps Performed

### 1. Launch EC2 Instance

* Selected Amazon Linux AMI
* Chose t3.micro (Free Tier)
* Created key pair (.pem)
* Allowed SSH (port 22) in security group

### 2. Connect to EC2

* Used EC2 Instance Connect (browser)
* Connected using SSH:
```
chmod 400 ec2Demo.pem
```
```
ssh -i ec2Demo.pem ec2-user@<my-public-ip>
```

### 3. Verified Access

* Successfully logged into EC2 instance
* Executed basic commands

---

## 📸 Screenshots

### EC2 Dashboard

![EC2 Dashboard](screenshots/ec2-dashboard.png)

### Security Group (Port 22 Open)

![Security Group](screenshots/security-group.png)

### EC2 Instance Connect

![EC2 Instance Connect](screenshots/ec2-instance-connect.png)

### SSH via Bash

![SSH Connection](screenshots/ssh-bash.png)

---

## 🧠 Key Learnings

* How to launch EC2 instance
* Importance of security groups (port 22 for SSH)
* Difference between browser access and SSH
* Connecting EC2 using key pair

---

## ⚠️ Common Issues Faced

* SSH timeout due to incorrect security group rules
* Permission issues with key file

---

## 🏁 Conclusion

Successfully launched and accessed an EC2 instance using multiple methods.
