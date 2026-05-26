# ☁️ AWS Fundamentals

# 🌐 AWS Global Infrastructure

AWS Global Infrastructure is the worldwide network of AWS data centers and networking resources.

It includes:
1. Regions
2. Availability Zones
3. Edge Locations

AWS infrastructure is designed for:
- High performance
- Security
- Reliability
- Fault tolerance

---

# 📌 Components of AWS Global Infrastructure

| Component | Description |
|---|---|
| Region | Geographic area containing AWS data centers |
| Availability Zone | Isolated data center inside a region |
| Edge Location | Used for faster content delivery |

---

# 🗺️ AWS Regions

An AWS Region is a physical geographic location where AWS maintains data centers.

## Examples of Regions
- Mumbai
- Singapore
- Tokyo
- London
- US East

Each region is isolated from other regions.

---

# ✅ Why Regions Are Important

Regions help:
- Reduce latency
- Improve speed
- Meet legal requirements
- Increase reliability

---

# 🌍 Real-Time Example

If Indian users use the Mumbai region:
- Website loads faster
- Response time becomes lower

If servers are in the US:
- Response may become slower due to distance.

---

# 📌 Important Points About Regions

- One region contains multiple Availability Zones.
- Users choose regions while creating AWS resources.
- Data can remain inside a country if required.

---

# 🏢 AWS Availability Zones (AZs)

An Availability Zone is one or more isolated data centers inside a region.

Each Availability Zone has:
- Independent power supply
- Networking
- Cooling systems
- Backup facilities

---

# 📍 Example

Mumbai Region may contain:
- ap-south-1a
- ap-south-1b
- ap-south-1c

These are Availability Zones.

---

# ✅ Why Availability Zones Are Important

Availability Zones improve:
- Fault tolerance
- Reliability
- High availability

If one data center fails, another AZ continues running the application.

---

# 🌍 Real-Time Example of Availability Zones

Suppose a website runs in:
- Availability Zone A

If power failure occurs:
- AWS automatically shifts traffic to another Availability Zone.

Users can still access the website.

---

# ⚖️ Difference Between Region and Availability Zone

| Region | Availability Zone |
|---|---|
| Geographic area | Data center inside region |
| Contains multiple AZs | Part of one region |
| Example: Mumbai | Example: ap-south-1a |

---

# 🏗️ Simple AWS Architecture Flow

```text
User → Internet → AWS Region → Availability Zone → AWS Services
```

---

# 🛠️ Common Beginner AWS Services

| Service | Purpose |
|---|---|
| EC2 | Virtual servers |
| S3 | Cloud storage |
| IAM | Security and access control |
| RDS | Managed database |
| CloudWatch | Monitoring and logging |

---

# 📝 Short Exam Definitions

## AWS
AWS is a cloud computing platform provided by Amazon that offers services such as servers, storage, networking, and databases over the internet.

---

## AWS Region
An AWS Region is a geographic location containing multiple AWS data centers.

---

## Availability Zone
An Availability Zone is an isolated data center inside an AWS Region designed for high availability and fault tolerance.

---

# 💡 Interview Questions

## What is AWS?
AWS is a cloud computing platform by Amazon that provides cloud services over the internet.

---

## What is an AWS Region?
A physical geographic area containing multiple Availability Zones.

---

## What is an Availability Zone?
An isolated data center inside a region used for high availability and backup.

---

## Why are Regions important?
Regions help reduce latency and improve application performance.

---

# 📚 Summary

- AWS is a cloud computing platform.
- AWS Global Infrastructure includes Regions and Availability Zones.
- Regions are geographic areas.
- Availability Zones are isolated data centers inside regions.
- AWS provides scalable, secure, and reliable cloud services.
