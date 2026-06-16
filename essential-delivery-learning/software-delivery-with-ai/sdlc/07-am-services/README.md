# 📘 Module 7: AMS Practices & Principles

## 🎯 Learning Objectives

At the end of this module, you will be able to:

* Understand AMS (Application Maintenance Services) practices.
* Explain Resolve and Control practices.
* Understand:

  * Incident Management
  * Problem Management
  * Service Request Management
  * Change Management
* Describe AM Engineer roles and responsibilities.

---

# 🚀 What is AMS?

**AMS (Application Maintenance Services)** refers to the support and maintenance activities performed after an application is deployed.

The goal of AMS is to ensure that applications remain:

* Available ✅
* Stable ⚙️
* Secure 🔒
* Efficient 🚀

---

# 🔄 AMS Workflow

```text id="m7flow"
User Reports Issue/Request
            ↓
      Incident Management
            ↓
      Problem Management
            ↓
      Change Management
            ↓
      Application Update
            ↓
      Continuous Monitoring
```

---

# 🛠️ AMS Practices

AMS practices are broadly divided into:

1. Resolve Practice
2. Control Practice

---

# 1️⃣ Resolve Practice

## What is Resolve Practice?

Resolve Practice focuses on **restoring services quickly** when issues occur.

### Objective

> Minimize downtime and restore normal operations.

### Activities

* Investigate incidents
* Fix application issues
* Communicate with users
* Restore services

### Example

A banking app server goes down.

The AMS team investigates and restores the service immediately.

---

# 2️⃣ Control Practice

## What is Control Practice?

Control Practice ensures that changes are implemented in a controlled and secure manner.

### Objective

> Reduce risks and maintain system stability.

### Activities

* Review changes
* Approve deployments
* Manage releases
* Maintain documentation

### Example

Before deploying a new feature, the team tests and approves it.

---

# 🚨 Incident Management

## What is Incident Management?

An **incident** is any unplanned interruption in service.

Incident Management aims to restore service as quickly as possible.

### Examples

* Application crash
* Login failure
* Server outage
* Payment failure

### Incident Lifecycle

```text id="incidentflow"
Incident Reported
        ↓
Classification
        ↓
Investigation
        ↓
Resolution
        ↓
Closure
```

### Goal

✅ Restore service quickly

---

# 🔍 Problem Management

## What is Problem Management?

Problem Management identifies the **root cause** of recurring incidents.

### Difference

* Incident = Fix immediate issue
* Problem = Find permanent solution

### Example

Users repeatedly face login failures.

The team discovers the root cause is a database issue and permanently fixes it.

### Goal

✅ Prevent incidents from recurring

---

# 📩 Service Request Management

## What is a Service Request?

A service request is a **user request for information or services**.

### Examples

* Password reset
* Access request
* Software installation
* Account creation

### Goal

✅ Fulfill user requests efficiently

---

# 🔄 Change Management

## What is Change Management?

Change Management ensures that changes to the application are implemented safely.

### Types of Changes

### Standard Change

Routine and low-risk changes.

**Example:** Password policy update.

### Normal Change

Requires approval and testing.

**Example:** Deploying a new feature.

### Emergency Change

Urgent fixes.

**Example:** Security patch after a cyber attack.

### Goal

✅ Minimize risks during changes

---

# 👨‍💻 AM Engineer Roles and Responsibilities

## Who is an AM Engineer?

An **Application Maintenance (AM) Engineer** supports and maintains applications after deployment.

---

## Responsibilities

### 🔧 Application Support

* Monitor applications
* Resolve incidents
* Ensure availability

### 🐞 Issue Resolution

* Analyze logs
* Troubleshoot problems
* Fix defects

### 📈 Performance Monitoring

* Monitor system health
* Improve performance
* Identify bottlenecks

### 🔄 Change Implementation

* Deploy updates
* Perform releases
* Follow change management processes

### 📚 Documentation

* Maintain knowledge base
* Document incidents and fixes

### 🤝 Communication

* Coordinate with developers
* Communicate with users
* Update stakeholders

---

# 🏥 Real-Life Analogy: Hospital

| AMS Concept                | Hospital Example          |
| -------------------------- | ------------------------- |
| Incident Management        | Treat patient immediately |
| Problem Management         | Diagnose root cause       |
| Service Request Management | Schedule appointment      |
| Change Management          | Introduce new treatment   |
| Resolve Practice           | Emergency care            |
| Control Practice           | Safety protocols          |

---

# 📌 Quick Revision

| Concept                    | Purpose                      |
| -------------------------- | ---------------------------- |
| Resolve Practice           | Restore service quickly      |
| Control Practice           | Manage changes safely        |
| Incident Management        | Handle service interruptions |
| Problem Management         | Remove root causes           |
| Service Request Management | Fulfill user requests        |
| Change Management          | Control modifications        |
| AM Engineer                | Maintain applications        |

---

# 🧠 Memory Trick

Remember:

**IPSC**

* **I** → Incident Management
* **P** → Problem Management
* **S** → Service Request Management
* **C** → Change Management

> **"Incidents Prevent Service Chaos."** 🚀

---

# ✅ Summary

AMS ensures that applications remain:

* Available ✅
* Stable ⚙️
* Secure 🔒
* Efficient 🚀

AM Engineers play a key role in maintaining software quality and user satisfaction.
