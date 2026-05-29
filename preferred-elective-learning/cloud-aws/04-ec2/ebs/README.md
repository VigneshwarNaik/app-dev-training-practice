# AWS Lab: Creating and Attaching Amazon EBS Volume to an EC2 Instance

## Introduction

In this lab, we will learn how to:

1. Create an Amazon EC2 Instance.
2. Create an Amazon EBS Volume.
3. Attach the EBS Volume to the EC2 Instance.

This lab helps us understand how storage works in AWS.

---

# What is Amazon EC2?

Amazon EC2 (Elastic Compute Cloud) is a service that provides virtual computers in the cloud.

Think of EC2 as:

```text
Your Personal Computer
     OR
A Virtual Server in AWS
```

An EC2 instance can:

* Run applications
* Host websites
* Store files
* Run databases

---

# What is Amazon EBS?

Amazon EBS (Elastic Block Store) is a storage service used with EC2.

Think of EBS as:

```text
Hard Disk of a Computer
```

Just like a laptop needs a hard disk to store data, an EC2 instance needs EBS to store:

* Operating System
* Applications
* Files
* Logs
* Databases

---

# Real Life Example

Imagine you buy a new laptop.

Laptop Components:

```text
Laptop = EC2 Instance

Hard Disk = EBS Volume
```

Without a hard disk:

```text
Laptop cannot store data
```

Without EBS:

```text
EC2 cannot store data
```

---

# Lab Architecture

```text
              AWS Cloud

                   │
                   ▼

          Amazon EC2 Instance
              (My Server)

                   │

         -------------------
         │                 │

         ▼                 ▼

   Root EBS Volume     New EBS Volume
      (8 GB)              (10 GB)

         │                 │

         ▼                 ▼

      Operating         Extra Storage
       System
```

---

# Task 1: Launch an EC2 Instance

## Step 1: Login to AWS

1. Open AWS Console.
2. Enter username.
3. Enter password.
4. Click Sign In.

You will see:

```text
AWS Management Console
```

---

## Step 2: Select Region

Select:

```text
Mumbai (ap-south-1)
```

Why?

Because all AWS resources will be created in this region.

---

## Step 3: Open EC2 Service

Go to:

```text
Services
→ EC2
```

EC2 Dashboard opens.

---

## Step 4: Launch Instance

Click:

```text
Launch Instance
```

---

## Step 5: Enter Instance Name

Type:

```text
My Server
```

Purpose:

To identify the server easily.

---

## Step 6: Select Operating System

Choose:

```text
Amazon Linux 2023
```

Amazon Linux is:

* Free
* Secure
* AWS Optimized

---

## Step 7: Select Instance Type

Choose:

```text
t3.micro
```

This is a small server suitable for:

* Practice
* Labs
* Learning AWS

Configuration:

```text
2 vCPU
1 GB RAM
```

---

## Step 8: Key Pair

For this lab:

```text
Proceed Without Key Pair
```

Normally:

A Key Pair is used to connect securely to the server.

---

## Step 9: Configure Network

Select:

```text
My VPC
```

Enable:

```text
Auto Assign Public IP
```

Why?

Because we want internet access.

---

## Step 10: Configure Security Group

Select:

```text
Default Security Group
```

Security Group acts like:

```text
Firewall
```

It controls who can access the server.

---

## Step 11: Configure Storage

Default Storage:

```text
8 GB gp3
```

This storage contains:

* Linux Operating System
* System Files

---

## Step 12: Launch Instance

Click:

```text
Launch Instance
```

AWS creates the virtual server.

---

## Step 13: Verify Instance

Go to:

```text
Instances
```

Wait until:

```text
Running
```

and

```text
2/2 Status Checks Passed
```

Meaning:

✅ AWS hardware is healthy

✅ Linux OS is healthy

---

# Task 2: Create an Additional EBS Volume

Now we create another hard disk.

---

## Step 1: Open Volumes

Go to:

```text
EC2
→ Elastic Block Store
→ Volumes
```

---

## Step 2: Create Volume

Click:

```text
Create Volume
```

---

## Step 3: Configure Volume

Volume Type:

```text
gp3
```

Size:

```text
10 GB
```

Availability Zone:

```text
ap-south-1a
```

Important:

The volume must be in the same Availability Zone as the EC2 instance.

---

## Step 4: Add Tag

Tag Key:

```text
Name
```

Tag Value:

```text
My Disk
```

Purpose:

Helps identify the volume.

---

## Step 5: Create Volume

Click:

```text
Create Volume
```

AWS creates a new EBS volume.

---

# Task 3: Attach EBS Volume to EC2

Now we connect the new hard disk to our server.

---

## Step 1: Open Volumes

Go to:

```text
EC2
→ Volumes
```

---

## Step 2: Select Volume

Choose:

```text
My Disk
```

---

## Step 3: Attach Volume

Click:

```text
Actions
→ Attach Volume
```

---

## Step 4: Select EC2 Instance

Choose:

```text
My Server
```

---

## Step 5: Device Name

Enter:

```text
/dev/sdb
```

This is the disk name Linux will use.

---

## Step 6: Click Attach

AWS connects the volume to the EC2 instance.

---

# Verification

Go to:

```text
Volumes
```

Check:

```text
State = In Use
```

Meaning:

```text
Volume successfully attached
```

---

# What Happened Internally?

Before:

```text
EC2 Server
    │
    ▼
8 GB Root Volume
```

After:

```text
EC2 Server
    │
    ├── 8 GB Root Volume
    │
    └── 10 GB New Volume
```

Now the server has extra storage.

---

# Advantages of EBS

### Persistent Storage

Data remains even if the server is stopped.

### Easy Expansion

Storage size can be increased later.

### Backup Support

Snapshots can be created.

### Secure

Supports encryption.

### Reliable

Data is replicated inside AWS.

---

# Interview Questions

## What is EC2?

EC2 is a virtual server in AWS.

---

## What is EBS?

EBS is a storage device attached to EC2.

---

## Difference Between EC2 and EBS?

| EC2               | EBS             |
| ----------------- | --------------- |
| Virtual Machine   | Storage Device  |
| Runs Applications | Stores Data     |
| Compute Service   | Storage Service |

---

## Why Do We Use EBS?

To store:

* Operating System
* Applications
* User Data
* Databases

---

## What is gp3?

A General Purpose SSD storage type used by EBS.

---

## Can an EBS Volume Exist Without EC2?

Yes.

EBS can be created independently and attached later.

---

## What Happens If EC2 Stops?

Data inside EBS remains safe because EBS is persistent storage.

---

# Conclusion

In this lab, we successfully:

✅ Created an EC2 Instance

✅ Created a 10 GB EBS Volume

✅ Attached the EBS Volume to the EC2 Instance

✅ Learned how AWS separates compute (EC2) and storage (EBS)

This is one of the most important AWS practicals because EBS is widely used in real-world cloud applications for storing operating systems, application data, databases, and backups.
