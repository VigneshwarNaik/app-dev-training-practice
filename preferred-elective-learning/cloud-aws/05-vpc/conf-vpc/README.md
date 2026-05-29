# Creating and Configuring a VPC (Virtual Private Cloud) in AWS

## Project Overview

This project demonstrates how to create and configure an Amazon VPC (Virtual Private Cloud) in AWS.

A VPC allows you to create your own private network inside AWS where you can launch resources such as EC2 instances, databases, and applications securely.

In this project, we will:

* Create a VPC
* Create an Internet Gateway
* Create Public and Private Subnets
* Create a Route Table
* Configure Internet Access
* Associate the Public Subnet with the Route Table

---

# Learning Objectives

After completing this project, you will be able to:

* Understand Amazon VPC
* Create a VPC
* Configure networking components
* Create Public and Private Subnets
* Configure Route Tables
* Connect a VPC to the Internet
* Understand AWS Networking Basics

---

# What is Amazon VPC?

Amazon VPC (Virtual Private Cloud) is a service that allows you to create a private network inside AWS.

Think of a VPC as your own private network where you can securely launch AWS resources.

### Simple Example

```text
Your House = VPC

Rooms = Subnets

Roads = Route Tables

Main Gate = Internet Gateway
```

---

# VPC Architecture

```text
                    Internet
                        │
                        ▼
                Internet Gateway
                   (DemoIGW)
                        │
                        ▼
                Route Table
                        │
                        ▼
      ----------------------------------
      |          DemoVPC               |
      |        10.0.0.0/16            |
      |                               |
      |  Public Subnet                |
      |  10.0.1.0/24                  |
      |                               |
      |  Private Subnet               |
      |  10.0.2.0/24                  |
      ----------------------------------
```

---

# Task 1: Create a VPC

## Step 1

Login to AWS Management Console.

## Step 2

Search for:

```text
VPC
```

Open the VPC Dashboard.

## Step 3

Click:

```text
Create VPC
```

## Step 4

Select:

```text
VPC Only
```

## Step 5

Enter the following details:

### Name

```text
DemoVPC
```

### IPv4 CIDR Block

```text
10.0.0.0/16
```

## Step 6

Click:

```text
Create VPC
```

### Result

A new VPC named DemoVPC is created.

---

# Understanding CIDR Block

CIDR block defines the IP address range available in the VPC.

Example:

```text
10.0.0.0/16
```

This provides thousands of private IP addresses for AWS resources.

---

# Task 2: Create an Internet Gateway

## What is an Internet Gateway?

An Internet Gateway allows communication between a VPC and the internet.

Without an Internet Gateway:

```text
EC2 Instance
     │
     ▼
No Internet Access
```

With an Internet Gateway:

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

## Steps

1. Open:

```text
Internet Gateways
```

2. Click:

```text
Create Internet Gateway
```

3. Enter Name:

```text
DemoIGW
```

4. Click:

```text
Create Internet Gateway
```

---

# Attach Internet Gateway to VPC

1. Select:

```text
DemoIGW
```

2. Click:

```text
Actions
→ Attach to VPC
```

3. Select:

```text
DemoVPC
```

4. Click:

```text
Attach Internet Gateway
```

### Result

The VPC is now connected to the internet.

---

# Task 3: Create a Public Subnet

## What is a Public Subnet?

A Public Subnet is a subnet that has internet access.

Usually used for:

* Web Servers
* Load Balancers

---

## Steps

1. Open:

```text
Subnets
```

2. Click:

```text
Create Subnet
```

3. Select VPC:

```text
DemoVPC
```

4. Enter:

### Subnet Name

```text
DemoPublicSubnet
```

### CIDR Block

```text
10.0.1.0/24
```

5. Click:

```text
Create Subnet
```

---

# Task 4: Create a Private Subnet

## What is a Private Subnet?

A Private Subnet does not have direct internet access.

Usually used for:

* Databases
* Internal Applications

---

## Steps

1. Click:

```text
Create Subnet
```

2. Select:

```text
DemoVPC
```

3. Enter:

### Subnet Name

```text
DemoPrivateSubnet
```

### CIDR Block

```text
10.0.2.0/24
```

4. Click:

```text
Create Subnet
```

---

# Public vs Private Subnet

| Public Subnet     | Private Subnet            |
| ----------------- | ------------------------- |
| Internet Access   | No Direct Internet Access |
| Web Servers       | Databases                 |
| Public IP Allowed | Private IP Only           |

---

# Task 5: Create a Route Table

## What is a Route Table?

A Route Table contains rules that decide where network traffic should go.

Think of it as:

```text
Google Maps for Network Traffic
```

---

## Steps

1. Open:

```text
Route Tables
```

2. Click:

```text
Create Route Table
```

3. Enter:

### Name

```text
DemoPublicRouteTable
```

### VPC

```text
DemoVPC
```

4. Click:

```text
Create Route Table
```

---

# Task 6: Add Internet Route

To allow internet access:

1. Select:

```text
DemoPublicRouteTable
```

2. Open:

```text
Routes
```

3. Click:

```text
Edit Routes
```

4. Click:

```text
Add Route
```

### Destination

```text
0.0.0.0/0
```

### Target

```text
DemoIGW
```

5. Save Changes.

---

# What Does 0.0.0.0/0 Mean?

```text
0.0.0.0/0
```

Means:

```text
All Internet Traffic
```

Send all internet traffic through the Internet Gateway.

---

# Task 7: Associate Public Subnet

Now connect the Public Subnet to the Route Table.

1. Select:

```text
DemoPublicRouteTable
```

2. Open:

```text
Subnet Associations
```

3. Click:

```text
Edit Subnet Associations
```

4. Select:

```text
DemoPublicSubnet
```

5. Save Changes.

### Result

The Public Subnet can now access the internet.

---

# Complete Network Flow

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
EC2 Instance
```

---

# Advantages of VPC

* Secure Network
* Private Environment
* Better Traffic Control
* Easy Resource Management
* Supports Public and Private Resources
* Highly Scalable

---

# AWS Services Used

* Amazon VPC
* Internet Gateway
* Route Tables
* Public Subnet
* Private Subnet

---

# Interview Questions

### What is Amazon VPC?

A private network inside AWS where resources can be launched securely.

### What is a Subnet?

A smaller network inside a VPC.

### What is a Public Subnet?

A subnet that has internet access.

### What is a Private Subnet?

A subnet without direct internet access.

### What is a Route Table?

A set of rules that controls network traffic.

### What is an Internet Gateway?

A service that connects a VPC to the internet.

### Why is 0.0.0.0/0 used?

It represents all internet traffic.

---

# Conclusion

In this project, we successfully created and configured an Amazon VPC named DemoVPC. We created Public and Private Subnets, attached an Internet Gateway, configured a Route Table, and enabled internet access for the Public Subnet. This setup is the foundation of AWS networking and is commonly used when deploying secure cloud applications.
