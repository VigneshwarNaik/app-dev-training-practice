# Amazon VPC (Virtual Private Cloud)

## Introduction

Amazon VPC (Virtual Private Cloud) is a service in AWS that allows you to create your own private network in the cloud.

Just like a company has its own office building and internal network, AWS allows you to create your own private network for your cloud resources.

Inside a VPC, you can launch:

* EC2 Instances
* Databases
* Applications
* Storage Services

---

# What is VPC?

VPC stands for:

```text
Virtual Private Cloud
```

### Simple Definition

A VPC is your own private network inside AWS.

It helps you control:

* Who can access your resources
* Which resources can connect to the internet
* How data travels inside the network

---

# Real Life Example

Imagine you build a house.

The house has:

```text
House = VPC

Rooms = Subnets

Roads = Route Tables

Main Gate = Internet Gateway
```

Just like a house needs rooms and roads, a VPC needs subnets and route tables.

---

# Why Do We Need VPC?

Without VPC:

```text
All resources are open to everyone.
```

With VPC:

```text
Resources stay inside a private network.
```

Benefits:

* Better Security
* Better Control
* Safe Communication
* Easy Management

---

# VPC Architecture

```text
                Internet
                    │
                    ▼
          Internet Gateway
                    │
                    ▼
               Amazon VPC
                    │
       ┌────────────┴────────────┐
       │                         │
       ▼                         ▼

 Public Subnet           Private Subnet

 EC2 Web Server          Database Server
```

---

# Private Cloud Networking

Private Cloud Networking means creating a private network inside AWS.

Only resources inside the VPC can communicate with each other unless permission is given.

Example:

```text
My VPC

├── Web Server
├── Application Server
└── Database Server
```

All these resources can communicate safely.

---

# CIDR Block

When creating a VPC, we assign an IP address range.

Example:

```text
10.0.0.0/16
```

This range provides IP addresses for resources inside the VPC.

Think of it as:

```text
Address range for your network
```

---

# Subnets

## What is a Subnet?

A Subnet is a smaller network inside a VPC.

### Simple Definition

A subnet is like a room inside a house.

---

# Why Use Subnets?

Subnets help organize resources.

Example:

```text
VPC

├── Public Subnet
└── Private Subnet
```

---

# Types of Subnets

## 1. Public Subnet

A Public Subnet has internet access.

Resources placed here:

* Web Servers
* Load Balancers

Example:

```text
Public Subnet

└── EC2 Web Server
```

Users can access these resources through the internet.

---

## 2. Private Subnet

A Private Subnet does not have direct internet access.

Resources placed here:

* Databases
* Internal Applications

Example:

```text
Private Subnet

└── Database Server
```

Users on the internet cannot access these resources directly.

---

# Public vs Private Subnet

| Public Subnet       | Private Subnet             |
| ------------------- | -------------------------- |
| Has Internet Access | No Direct Internet Access  |
| Stores Web Servers  | Stores Databases           |
| Accessible by Users | Accessible Only Internally |

---

# Route Tables

## What is a Route Table?

A Route Table is a set of rules that decides where network traffic should go.

### Simple Definition

A Route Table is like Google Maps for network traffic.

It tells data:

```text
Where to go next
```

---

# Example

Suppose a user requests a website.

The Route Table decides:

```text
User Request
      │
      ▼
Route Table
      │
      ▼
Web Server
```

---

# Common Route

```text
0.0.0.0/0 → Internet Gateway
```

Meaning:

```text
Send all internet traffic to the Internet Gateway.
```

---

# Internet Gateway

## What is an Internet Gateway?

An Internet Gateway is a service that connects a VPC to the internet.

### Simple Definition

An Internet Gateway is the main gate of your network.

---

# Why Do We Need Internet Gateway?

Without Internet Gateway:

```text
EC2 Instance
     │
     ▼
Cannot Access Internet
```

With Internet Gateway:

```text
EC2 Instance
     │
     ▼
Internet Gateway
     │
     ▼
Internet
```

---

# Example

Suppose your website is hosted on EC2.

User Flow:

```text
User
 │
 ▼
Internet
 │
 ▼
Internet Gateway
 │
 ▼
Public Subnet
 │
 ▼
EC2 Web Server
```

Without Internet Gateway, users cannot open the website.

---

# Complete VPC Flow

```text
User
 │
 ▼
Internet
 │
 ▼
Internet Gateway
 │
 ▼
Route Table
 │
 ▼
Public Subnet
 │
 ▼
EC2 Web Server
 │
 ▼
Private Subnet
 │
 ▼
Database
```

---

# Advantages of VPC

* Secure Network
* Private Environment
* Better Control
* Easy Management
* Safe Communication
* Supports Public and Private Resources

---

# Interview Questions

### What is VPC?

A VPC is a private network inside AWS where resources can be launched securely.

### What is a Subnet?

A subnet is a smaller network inside a VPC.

### What is a Public Subnet?

A subnet that has internet access.

### What is a Private Subnet?

A subnet that does not have direct internet access.

### What is a Route Table?

A Route Table decides where network traffic should go.

### What is an Internet Gateway?

An Internet Gateway connects a VPC to the internet.

### Why do we use VPC?

To create a secure and private network for AWS resources.

---

# Conclusion

Amazon VPC is a private network inside AWS. Inside a VPC, we create Subnets to organize resources, Route Tables to control traffic, and Internet Gateways to provide internet access. Together, these components help build secure and scalable cloud networks.
