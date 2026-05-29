# AWS Security and Compliance Services

## Introduction

Security is very important in cloud computing because organizations store important data and applications in the cloud.

AWS provides many security services to:

* Protect data
* Protect applications
* Control user access
* Monitor activities
* Detect threats
* Meet compliance requirements

These services help keep AWS resources safe and secure.

---

# What is Security?

Security means protecting AWS resources from unauthorized access.

Examples:

* Protecting passwords
* Protecting data
* Protecting servers
* Preventing cyber attacks

---

# What is Compliance?

Compliance means following rules and standards set by governments or organizations.

Examples:

* GDPR
* HIPAA
* ISO 27001
* PCI DSS

AWS provides tools that help companies follow these standards.

---

# AWS Shared Responsibility Model

AWS and customers share security responsibilities.

### AWS is Responsible For

```text id="r2l5uo"
Data Centers
Servers
Networking
Hardware
```

### Customer is Responsible For

```text id="bzlq3y"
Data
Passwords
Applications
User Permissions
```

---

# Main AWS Security Services

## 1. IAM (Identity and Access Management)

### What is IAM?

IAM controls who can access AWS resources.

Think of IAM as:

```text id="0zx5kq"
Security Guard of AWS
```

IAM allows you to:

* Create Users
* Create Groups
* Assign Permissions
* Control Access

### Example

```text id="gvrz0o"
Admin User
Developer User
Tester User
```

Each user gets different permissions.

---

# 2. AWS Shield

### What is AWS Shield?

AWS Shield protects websites and applications from DDoS attacks.

### What is a DDoS Attack?

A DDoS attack sends huge amounts of traffic to crash a website.

Example:

```text id="6fb8ns"
Millions of Requests
         │
         ▼
      Website
         │
         ▼
      Website Crash
```

AWS Shield blocks these attacks.

---

# 3. AWS WAF (Web Application Firewall)

### What is AWS WAF?

AWS WAF protects websites from harmful requests.

Think of WAF as:

```text id="m4tbpq"
Security Checkpoint
```

Before users enter a website, WAF checks their requests.

It protects against:

* SQL Injection
* Cross-Site Scripting (XSS)
* Bots
* Malicious Traffic

---

# 4. AWS KMS (Key Management Service)

### What is KMS?

AWS KMS is used to encrypt data.

### What is Encryption?

Encryption converts data into secret code.

Example:

```text id="9jdfbn"
Original Data
      │
      ▼
Encryption
      │
      ▼
Secret Data
```

Only authorized users can read it.

---

# 5. AWS Secrets Manager

### What is Secrets Manager?

Secrets Manager stores sensitive information securely.

Examples:

```text id="7ccq6w"
Database Passwords
API Keys
Access Tokens
```

Instead of storing passwords in code, they are stored safely in Secrets Manager.

---

# 6. AWS CloudTrail

### What is CloudTrail?

CloudTrail records all activities performed in AWS.

Think of it as:

```text id="8rkq7e"
AWS Activity History
```

It records:

* Login Activities
* EC2 Creation
* S3 Uploads
* Configuration Changes

### Example

```text id="vr7lkl"
User Created EC2
      │
      ▼
CloudTrail Records Event
```

---

# 7. Amazon GuardDuty

### What is GuardDuty?

GuardDuty continuously monitors AWS accounts for threats.

It detects:

* Suspicious Logins
* Malware
* Unusual Activities

### Example

```text id="ww8vr4"
Unknown User Login
        │
        ▼
GuardDuty Alert
```

---

# 8. AWS Inspector

### What is AWS Inspector?

Inspector scans AWS resources and finds security problems.

It checks:

* EC2 Instances
* Applications
* Containers

### Purpose

```text id="ckd7ov"
Find Security Weaknesses
```

before attackers do.

---

# 9. AWS Config

### What is AWS Config?

AWS Config tracks changes made to AWS resources.

It answers:

```text id="d8t63h"
Who changed it?

When was it changed?

What was changed?
```

Useful for auditing and troubleshooting.

---

# 10. AWS Artifact

### What is AWS Artifact?

AWS Artifact provides compliance reports and security documents.

Examples:

```text id="y0ub79"
ISO Reports
SOC Reports
PCI Reports
```

Companies use these reports during audits.

---

# Security Services Overview

| Service         | Purpose                      |
| --------------- | ---------------------------- |
| IAM             | Manage Users and Permissions |
| Shield          | Protect from DDoS Attacks    |
| WAF             | Protect Websites             |
| KMS             | Encrypt Data                 |
| Secrets Manager | Store Passwords Securely     |
| CloudTrail      | Record AWS Activities        |
| GuardDuty       | Detect Threats               |
| Inspector       | Find Security Issues         |
| Config          | Track Configuration Changes  |
| Artifact        | Compliance Reports           |

---

# Easy Memory Trick

```text id="7k1qec"
IAM            → Who Can Access?

Shield         → Protect Website from DDoS

WAF            → Filter Bad Requests

KMS            → Encrypt Data

Secrets Manager → Store Passwords

CloudTrail     → Record Activities

GuardDuty      → Detect Threats

Inspector      → Find Vulnerabilities

Config         → Track Changes

Artifact       → Compliance Reports
```

---

# Interview Questions

### What is IAM?

IAM controls user access and permissions in AWS.

### What is AWS Shield?

AWS Shield protects applications from DDoS attacks.

### What is AWS WAF?

AWS WAF protects websites from malicious traffic.

### What is KMS?

KMS is used to encrypt data.

### What is CloudTrail?

CloudTrail records all AWS activities.

### What is GuardDuty?

GuardDuty detects suspicious activities and threats.

### What is AWS Config?

AWS Config tracks resource changes.

### What is AWS Artifact?

AWS Artifact provides compliance reports.

---

# Conclusion

AWS provides many security and compliance services to protect cloud resources. IAM controls access, Shield protects against attacks, WAF secures websites, KMS encrypts data, CloudTrail records activities, GuardDuty detects threats, Inspector finds vulnerabilities, Config tracks changes, and Artifact provides compliance reports. Together, these services help keep AWS environments secure and compliant.
