# AWS EC2 Static Website Deployment

## Project Overview
This project demonstrates how to deploy a static website on an AWS EC2 Ubuntu instance using Nginx.

## Technologies Used
- AWS EC2
- Ubuntu Linux
- Nginx
- SSH
- Security Groups
- HTML

## Steps Performed

### 1. Launch EC2 Instance
- Ubuntu Server
- t3.micro
- Public IP enabled

### 2. Configure Security Group
- SSH (22)
- HTTP (80)

### 3. Connect to EC2

```bash
ssh -i key.pem ubuntu@<public-ip>
