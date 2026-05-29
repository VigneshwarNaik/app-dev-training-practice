# Amazon EC2 (Elastic Compute Cloud)

## Introduction

Amazon EC2 (Elastic Compute Cloud) is one of the most important services provided by Amazon Web Services (AWS).

EC2 allows users to create and run virtual servers in the cloud. These virtual servers are called **Instances**.

Instead of purchasing and maintaining physical computers, organizations can launch virtual machines on AWS and pay only for the resources they use.

Amazon EC2 provides secure, scalable, and resizable computing capacity that helps developers deploy applications quickly and efficiently.

---

# What is Amazon EC2?

Amazon EC2 stands for:

```text
Elastic Compute Cloud
```

### Meaning

* **Elastic** → Resources can be increased or decreased when needed.
* **Compute** → Provides processing power (CPU and Memory).
* **Cloud** → Resources are available over the internet.

EC2 allows users to run applications without purchasing physical hardware.

---

# Why Do We Use EC2?

Traditionally, companies needed:

* Physical servers
* Data centers
* Network equipment
* Maintenance teams

These resources are expensive and difficult to manage.

With Amazon EC2:

* No physical hardware is required.
* Servers can be created in minutes.
* Resources can be scaled up or down.
* Users pay only for what they use.

---

# Real-Life Example

Imagine you want to host a website.

Without AWS:

```text
Buy Server
     ↓
Install Operating System
     ↓
Configure Network
     ↓
Deploy Website
```

With AWS EC2:

```text
Launch EC2 Instance
     ↓
Install Web Server
     ↓
Deploy Website
```

This process takes only a few minutes.

---

# Features of Amazon EC2

## 1. Scalability

EC2 resources can be increased or decreased according to workload.

Example:

```text
Normal Traffic → Small Instance

High Traffic → Large Instance
```

---

## 2. Flexibility

Users can choose:

* Operating System
* CPU
* Memory
* Storage
* Network Settings

---

## 3. Security

EC2 provides:

* Security Groups
* Key Pairs
* IAM Integration
* Network Isolation

---

## 4. Cost Effective

Users pay only for:

```text
Resources Used
```

No need to purchase expensive hardware.

---

## 5. High Availability

EC2 instances can be launched across multiple AWS Regions and Availability Zones.

---

# EC2 Architecture

```text
                  User
                    │
                    ▼
              Internet
                    │
                    ▼
             Public IP Address
                    │
                    ▼
             Security Group
                    │
                    ▼
             EC2 Instance
                    │
                    ▼
            Operating System
                    │
                    ▼
              Application
```

---

# Components of Amazon EC2

## 1. Instance

An Instance is a virtual machine running in AWS.

Example:

```text
MyWebServer
```

An instance contains:

* CPU
* RAM
* Storage
* Operating System

---

## 2. Amazon Machine Image (AMI)

An AMI is a template used to create an EC2 instance.

It contains:

* Operating System
* Software Packages
* Configuration Settings

Examples:

```text
Amazon Linux 2023
Ubuntu
Windows Server
Red Hat Linux
```

---

## 3. Instance Type

Instance Types define the hardware configuration.

Example:

```text
t3.micro
```

Specifications:

```text
2 vCPU
1 GB RAM
```

Popular Types:

| Instance Type | Purpose              |
| ------------- | -------------------- |
| t3.micro      | Learning             |
| t3.small      | Small Applications   |
| t3.medium     | Medium Applications  |
| m5.large      | Production Workloads |

---

## 4. Key Pair

A Key Pair is used for secure login.

Components:

### Public Key

Stored in AWS.

### Private Key

Downloaded by the user.

Example:

```text
mywebserver-key.pem
```

---

## 5. Security Group

A Security Group acts as a virtual firewall.

Controls:

* Inbound Traffic
* Outbound Traffic

Example Rules:

| Port | Protocol | Purpose               |
| ---- | -------- | --------------------- |
| 22   | SSH      | Remote Access         |
| 80   | HTTP     | Website Access        |
| 443  | HTTPS    | Secure Website Access |

---

## 6. Elastic IP

Elastic IP is a static public IP address.

Benefits:

* Permanent IP
* Can be reassigned to other instances

---

## 7. EBS Volume

EBS (Elastic Block Store) provides storage for EC2.

Think of EBS as:

```text
Hard Disk of a Computer
```

Stores:

* Operating System
* Applications
* Data

---

# EC2 Instance Lifecycle

```text
Launch
   ↓
Pending
   ↓
Running
   ↓
Stopping
   ↓
Stopped
   ↓
Starting
   ↓
Running
   ↓
Terminated
```

### Running

Instance is active.

### Stopped

Instance is powered off.

### Terminated

Instance is permanently deleted.

---

# Steps to Launch an EC2 Instance

## Step 1

Login to AWS Console.

---

## Step 2

Open EC2 Dashboard.

```text
Services
→ EC2
```

---

## Step 3

Click:

```text
Launch Instance
```

---

## Step 4

Enter Instance Name.

Example:

```text
MyWebServer
```

---

## Step 5

Select AMI.

Example:

```text
Amazon Linux 2023
```

---

## Step 6

Select Instance Type.

Example:

```text
t3.micro
```

---

## Step 7

Create or Select Key Pair.

---

## Step 8

Configure Security Group.

Allow:

```text
SSH (22)
HTTP (80)
HTTPS (443)
```

---

## Step 9

Configure Storage.

Example:

```text
8 GB gp3
```

---

## Step 10

Click:

```text
Launch Instance
```

AWS creates the virtual server.

---

# Advantages of EC2

* Easy to use
* Highly scalable
* Cost effective
* Secure
* Flexible
* Reliable
* Global availability

---

# Limitations

* Requires cloud knowledge
* Costs increase with large workloads
* User is responsible for server management

---

# Common Use Cases

## Website Hosting

Host static and dynamic websites.

## Application Hosting

Run business applications.

## Testing and Development

Create temporary environments.

## Machine Learning

Train AI and ML models.

## Database Servers

Host databases.

## Big Data Processing

Analyze large datasets.

---

# Interview Questions

### What is Amazon EC2?

Amazon EC2 is a cloud service that provides virtual servers called instances.

---

### What is an Instance?

An Instance is a virtual machine running in AWS.

---

### What is an AMI?

An Amazon Machine Image used to create EC2 instances.

---

### What is a Security Group?

A virtual firewall controlling network traffic.

---

### What is a Key Pair?

A secure authentication mechanism used to connect to EC2 instances.

---

### What is an Elastic IP?

A static public IP address assigned to an EC2 instance.

---

### What is EBS?

Elastic Block Store is persistent storage attached to EC2.

---

### What is the difference between EC2 and EBS?

| EC2               | EBS             |
| ----------------- | --------------- |
| Compute Service   | Storage Service |
| Virtual Machine   | Virtual Disk    |
| Runs Applications | Stores Data     |

---

# Conclusion

Amazon EC2 is one of the core AWS services that provides scalable virtual servers in the cloud. It enables organizations to deploy applications quickly, reduce infrastructure costs, and scale resources according to demand. Understanding EC2 concepts such as Instances, AMIs, Security Groups, Key Pairs, and EBS Volumes is essential for AWS Cloud Practitioner, AWS Solutions Architect, and cloud engineering roles.
