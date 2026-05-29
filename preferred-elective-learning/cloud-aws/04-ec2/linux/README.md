# Create an Amazon EC2 Instance (Linux) and Deploy a Sample Web Application

## Project Overview

This project demonstrates how to create an Amazon EC2 Linux instance, configure networking and security settings, install a web server, and deploy a sample web application accessible from the internet.

Amazon EC2 (Elastic Compute Cloud) is one of the core AWS services that provides virtual servers in the cloud. Instead of purchasing physical hardware, organizations can launch virtual machines on demand and pay only for the resources they use.

In this project, we will:

* Launch an Amazon EC2 Linux instance
* Configure Security Groups
* Connect to the instance
* Install Apache Web Server
* Deploy a sample website
* Access the website through a browser

---

# Learning Objectives

After completing this project, you will be able to:

* Understand Amazon EC2 architecture
* Create and launch Linux instances
* Configure Security Groups and networking
* Understand VPC and Subnets
* Connect to EC2 using EC2 Instance Connect
* Install and manage Apache HTTP Server
* Deploy static web pages
* Access applications through a Public IP Address
* Troubleshoot common EC2 deployment issues

---

# What is Amazon EC2?

Amazon EC2 (Elastic Compute Cloud) is a service that provides scalable computing resources in the AWS cloud.

EC2 allows users to:

* Launch virtual machines
* Install software
* Host websites
* Run applications
* Create development environments
* Deploy enterprise solutions

### Real World Example

Suppose a company wants to host a website.

Traditionally they would need:

* Physical server
* Data center
* Network equipment
* Maintenance team

Using EC2:

* AWS provides virtual servers instantly
* No hardware purchase required
* Pay only for usage
* Scale resources as needed

---

# EC2 Architecture

```text
                  Internet
                      │
                      ▼
               Public IP Address
                      │
                      ▼
               Security Group
                      │
                      ▼
                 Amazon EC2
                      │
                      ▼
             Amazon Linux 2023
                      │
                      ▼
             Apache HTTP Server
                      │
                      ▼
               index.html Page
                      │
                      ▼
                User Browser
```

---

# AWS Services Used

## Amazon EC2

Provides virtual servers.

## Security Groups

Acts as a firewall.

## VPC

Virtual network environment.

## Public IPv4 Address

Allows internet access.

## Amazon Linux 2023

Operating system used in the instance.

---

# Prerequisites

Before starting:

* AWS Account
* Internet Connection
* AWS Management Console Access
* Basic Linux knowledge

---

# Step 1: Login to AWS Management Console

1. Open AWS Console.
2. Enter credentials.
3. Sign in.

After successful login:

```text
AWS Management Console Dashboard
```

appears.

---

# Step 2: Open Amazon EC2 Service

Navigate:

```text
Services
→ Compute
→ EC2
```

The EC2 Dashboard appears.

---

# Step 3: Launch an EC2 Instance

Click:

```text
Launch Instance
```

---

# Step 4: Configure Instance Name

Instance Name:

```text
MyWebServer
```

Purpose:

Helps identify the server among multiple instances.

---

# Step 5: Select Amazon Machine Image (AMI)

### What is an AMI?

AMI (Amazon Machine Image) is a template containing:

* Operating System
* System Software
* Configuration Settings

Select:

```text
Amazon Linux 2023
```

Benefits:

* AWS optimized
* Secure
* Free Tier eligible
* Long-term support

---

# Step 6: Select Instance Type

Choose:

```text
t3.micro
```

Specifications:

| Resource | Value |
| -------- | ----- |
| vCPU     | 2     |
| Memory   | 1 GiB |
| Storage  | EBS   |

Purpose:

Suitable for:

* Practice
* Labs
* Small websites
* Learning AWS

---

# Step 7: Create Key Pair

### Why Key Pair is Needed

A Key Pair is used for secure login.

Components:

| Component   | Purpose            |
| ----------- | ------------------ |
| Public Key  | Stored on AWS      |
| Private Key | Downloaded by User |

Create:

```text
mywebserver-key
```

Format:

```text
.pem
```

Store safely.

---

# Step 8: Configure Network Settings

### Auto Assign Public IP

Enable:

```text
Auto Assign Public IP
```

Purpose:

Allows users to access the server through the internet.

---

# Step 9: Configure Security Group

### What is Security Group?

A Security Group acts as a virtual firewall.

### Required Rules

#### SSH

```text
Port: 22
Source: Anywhere
```

Purpose:

Remote server access.

#### HTTP

```text
Port: 80
Source: Anywhere
```

Purpose:

Website access.

#### HTTPS

```text
Port: 443
Source: Anywhere
```

Purpose:

Secure website access.

---

# Step 10: Configure Storage

Default Storage:

```text
8 GiB gp3
```

Purpose:

Stores:

* Operating System
* Website Files
* Applications
* Logs

---

# Step 11: Launch Instance

Click:

```text
Launch Instance
```

AWS provisions the virtual machine.

---

# Step 12: Verify Instance Status

Navigate:

```text
Instances
```

Check:

```text
Instance State = Running
```

and

```text
Status Check = 2/2 Checks Passed
```

### Meaning of Status Checks

#### System Status Check

AWS hardware is healthy.

#### Instance Status Check

Operating system is healthy.

---

# Step 13: Connect to the Instance

Select Instance.

Click:

```text
Connect
```

Choose:

```text
EC2 Instance Connect
```

Click:

```text
Connect
```

Terminal opens:

```bash
[ec2-user@ip-172-31-x-x ~]$
```

---

# Step 14: Update Linux Packages

Run:

```bash
sudo dnf update -y
```

Purpose:

* Installs updates
* Fixes bugs
* Improves security

---

# Step 15: Install Apache Web Server

Run:

```bash
sudo dnf install httpd -y
```

Apache HTTP Server is installed.

---

# Step 16: Start Apache Service

Start:

```bash
sudo systemctl start httpd
```

Enable automatic startup:

```bash
sudo systemctl enable httpd
```

Verify:

```bash
sudo systemctl status httpd
```

Expected:

```text
active (running)
```

---

# Step 17: Test Apache Installation

Open Browser:

```text
http://PUBLIC-IP
```

Example:

```text
http://18.234.174.18
```

You should see:

```text
Apache Test Page
```

---

# Step 18: Deploy Sample Web Application

Navigate:

```bash
cd /var/www/html
```

Create webpage:

```bash
sudo nano index.html
```

Paste:

```html
<!DOCTYPE html>
<html>
<head>
<title>AWS EC2 Web Server</title>
</head>

<body>

<h1>Welcome to AWS EC2</h1>

<h2>My First Web Application</h2>

<p>Hosted on Amazon EC2 Linux Instance</p>

</body>
</html>
```

Save:

```text
CTRL + X
Y
ENTER
```

---

# Step 19: Verify Deployment

Open Browser:

```text
http://PUBLIC-IP
```

Example:

```text
http://18.234.174.18
```

Output:

```text
Welcome to AWS EC2
My First Web Application
Hosted on Amazon EC2 Linux Instance
```

---

# Common Linux Commands

### List Files

```bash
ls
```

### Current Directory

```bash
pwd
```

### Change Directory

```bash
cd
```

### View File

```bash
cat index.html
```

### Edit File

```bash
nano index.html
```

---

# Troubleshooting

## Website Not Opening

Check:

```bash
sudo systemctl status httpd
```

---

## Connection Timed Out

Verify Security Group:

```text
HTTP Port 80 Enabled
```

---

## Permission Denied

Use:

```bash
sudo
```

before commands.

---

# Interview Questions

### What is Amazon EC2?

Amazon EC2 is a cloud service that provides virtual servers for running applications.

### What is an AMI?

A preconfigured operating system template used to launch EC2 instances.

### What is a Security Group?

A virtual firewall controlling inbound and outbound traffic.

### What is a Key Pair?

A secure authentication mechanism used to connect to EC2 instances.

### Why is Port 80 opened?

To allow web traffic.

### Why is Port 22 opened?

To allow SSH access.

### What does 2/2 status checks passed mean?

The instance and AWS infrastructure are healthy.

### Where are Apache website files stored?

```text
/var/www/html
```

### What is the difference between EC2 and S3?

| EC2                   | S3                       |
| --------------------- | ------------------------ |
| Virtual Server        | Object Storage           |
| Supports Dynamic Apps | Supports Static Websites |
| Has Operating System  | No Operating System      |
| Can Run Apache        | Cannot Run Apache        |

---

# Conclusion

In this project, we successfully launched an Amazon EC2 Linux instance, configured networking and security settings, installed the Apache web server, and deployed a sample web application. This project provides hands-on experience with core AWS services and demonstrates how cloud-based virtual servers can be used to host web applications efficiently.
