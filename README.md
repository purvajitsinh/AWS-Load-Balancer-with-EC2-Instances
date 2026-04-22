# AWS Load Balancer with EC2 Instances

## 📌 Project Overview
This project demonstrates how to deploy a scalable web application using AWS EC2 instances and an Application Load Balancer. Traffic is distributed across multiple servers to ensure high availability and reliability.

---

## 🛠️ Services Used
- AWS EC2 (Elastic Compute Cloud)
- Application Load Balancer (ALB)
- Target Group
- Amazon Linux
- Apache (httpd)

---

## 🚀 Project Architecture
Users → Load Balancer → EC2 Instance 1  
                         → EC2 Instance 2  

---

## ⚙️ Setup Steps

### 1. Launch EC2 Instances
- Created 2 EC2 instances using Amazon Linux  
- Allowed ports 22 (SSH) and 80 (HTTP)  

### 2. Configure Web Server
- Installed Apache (httpd)  
- Started and enabled the service  
- Deployed simple HTML pages  

### 3. Create Target Group
- Added both EC2 instances  
- Configured health checks on port 80  

### 4. Create Load Balancer
- Created an Application Load Balancer  
- Configured listener on HTTP (port 80)  
- Connected to target group  

### 5. Test Application
- Accessed the Load Balancer DNS  
- Verified traffic distribution between servers  

---

## 📂 Project Files
- `setup-commands.txt` → Contains all commands used for server setup  

---

## 📸 Output
- Successfully deployed a load-balanced web application  
- Traffic distributed between multiple EC2 instances  

---

## 💡 Key Learnings
- Load balancing and high availability  
- AWS networking and security groups  
- EC2 server management  
- Real-world cloud deployment  

---

## 🔗 Future Improvements
- Add Auto Scaling  
- Use HTTPS with SSL certificate  
- Integrate CloudFront CDN  
