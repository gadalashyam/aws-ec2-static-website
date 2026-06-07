# AWS EC2 Static Website Deployment

## Project URL

https://roadmap.sh/projects/ec2-instance

## Project Overview

This project demonstrates the deployment of a static website on an AWS EC2 Ubuntu instance using Nginx.

## Technologies Used

* AWS EC2
* Ubuntu Linux
* Nginx
* SSH
* Security Groups
* HTML

## Architecture

User Browser → AWS EC2 (Ubuntu) → Nginx Web Server → Static HTML Website

## Implementation Steps

### 1. Launch EC2 Instance

* Selected Ubuntu Server AMI
* Chose t2.micro instance type
* Enabled Public IP

### 2. Configure Security Group

* SSH (Port 22)
* HTTP (Port 80)

### 3. Connect to EC2

```bash
ssh -i my-key.pem ubuntu@<public-ip>
```

### 4. Install Nginx

```bash
sudo apt update
sudo apt install nginx -y
sudo systemctl enable nginx
sudo systemctl start nginx
```

### 5. Deploy Website

```bash
sudo nano /var/www/html/index.html
```

Copied the website code and saved the file.

### 6. Verify Deployment

```bash
http://<public-ip>
```

Successfully hosted a static website on AWS EC2 using Nginx.

## Project Outcomes

* Gained hands-on experience with AWS EC2.
* Learned Linux server administration.
* Configured Security Groups and SSH access.
* Installed and managed Nginx.
* Hosted a static website in the cloud.
