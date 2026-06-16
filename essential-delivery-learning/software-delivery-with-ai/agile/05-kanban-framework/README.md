# Module 5 – Kanban Framework

## 📌 Overview

This module introduces **Kanban**, an Agile framework used to visualize work, manage workflow, and improve team efficiency.

Kanban helps teams:

* Visualize tasks
* Limit work in progress
* Improve workflow
* Deliver work continuously

> **Kanban = Visualize Work + Limit Work + Improve Flow**

---

## 🎯 Learning Outcomes

At the end of this module, you will be able to:

* Explain the Kanban framework
* Describe Kanban features and benefits
* Describe the Kanban workflow
* Explain Kanban visualization techniques
* Understand the importance of Work-In-Progress (WIP) limits
* Explain flow management and policies
* Understand Kanban metrics

---

# 1. What is Kanban?

**Kanban** is a visual workflow management method that helps teams improve efficiency by managing and tracking work.

The word **Kanban** means **"visual board"** in Japanese.

---

# 2. Kanban Board

A Kanban board shows the status of tasks.

Example:

```text id="f2g8kp"
To Do → In Progress → Testing → Done
```

Tasks move from left to right as work progresses.

---

# 3. Example: Food Delivery App

Suppose we are building a **Food Delivery App**.

Tasks:

* Login
* Search Restaurants
* Payment
* Notifications

Kanban Board:

```text id="z1v4mq"
To Do:
- Payment
- Notifications

In Progress:
- Search Restaurants

Done:
- Login
```

By looking at the board, everyone knows:

* What is pending
* What is in progress
* What is completed

---

# 4. Kanban Workflow

Work flows continuously through stages.

```text id="h9n5rt"
Backlog → To Do → In Progress → Testing → Done
```

Unlike Scrum, Kanban does **not** use fixed Sprints.

New tasks can be added anytime.

---

# 5. Kanban Features

## Visual Management

Work is displayed visually using cards and boards.

Example:

```text id="d6w1sa"
Task: Payment Module
Status: In Progress
```

---

## Continuous Flow

Tasks move continuously through the workflow.

No waiting for sprint completion.

---

## Pull System

Team members pull new work when they have capacity.

Example:

```text id="r4q8yt"
Finish Login
      ↓
Pull Payment Task
```

---

# 6. Work-In-Progress (WIP) Limits

**WIP Limit** = Maximum number of tasks allowed in a stage.

Example:

```text id="j5m2lx"
In Progress Limit = 2
```

If two tasks are already in progress:

❌ Do not start a third task.

Complete existing work first.

---

## Why WIP Limits?

Without WIP Limits:

```text id="s8v6pc"
10 tasks started
0 tasks completed
```

With WIP Limits:

```text id="m3r9zn"
2 tasks started
2 tasks completed
```

Benefits:

* Better focus
* Faster completion
* Reduced multitasking

---

# 7. Flow Management

Kanban focuses on smooth workflow.

Goal:

```text id="k7t4qx"
Reduce waiting time
Improve delivery speed
```

### Example

If too many tasks are waiting for testing:

```text id="u2y5wr"
Development → Waiting → Testing
```

Testing becomes a bottleneck.

The team improves the testing process.

---

# 8. Explicit Policies

Policies define how work moves through the system.

Examples:

```text id="p1n8vd"
✓ Code review required
✓ Testing must pass
✓ Approval needed before deployment
```

Policies ensure consistency and quality.

---

# 9. Kanban Metrics

Metrics help measure performance.

---

## Lead Time

Time from request to completion.

Example:

```text id="g6k3xp"
Requested: Monday
Completed: Friday

Lead Time = 5 days
```

---

## Cycle Time

Time spent actively working on a task.

Example:

```text id="q4b7mt"
Started: Wednesday
Finished: Friday

Cycle Time = 2 days
```

---

## Throughput

Number of tasks completed during a period.

Example:

```text id="w9c2rz"
Tasks completed this week = 10
```

Throughput = **10 tasks/week**

---

# 10. Cumulative Flow Diagram (CFD)

A **Cumulative Flow Diagram (CFD)** shows how tasks move through different workflow stages.

CFD helps identify:

* Bottlenecks
* Delays
* Workflow efficiency

Example:

Too many tasks in **Testing** indicate a bottleneck.

---

# 11. Kanban vs Scrum

| Feature    | Kanban     | Scrum         |
| ---------- | ---------- | ------------- |
| Sprints    | No         | Yes           |
| Workflow   | Continuous | Sprint-based  |
| Roles      | Flexible   | Defined Roles |
| WIP Limits | Yes        | Usually No    |
| Changes    | Anytime    | Next Sprint   |

---

# 12. Benefits of Kanban

✅ Visualize work clearly

✅ Improve productivity

✅ Reduce bottlenecks

✅ Deliver continuously

✅ Increase team efficiency

✅ Improve workflow transparency

---

# 🔑 Key Takeaways

* Kanban is a visual workflow management framework.
* Work is tracked using a **Kanban Board**.
* Tasks move through stages continuously.
* **WIP Limits** prevent overloading the team.
* Metrics like **Lead Time**, **Cycle Time**, and **Throughput** measure performance.
* Kanban improves flow and productivity.

---

# 📝 Quick Quiz

### Q1. What is Kanban?

**Answer:**
A visual workflow management method used to improve efficiency.

---

### Q2. What is a Kanban Board?

**Answer:**
A board that visualizes task status.

---

### Q3. What is WIP?

**Answer:**
Work-In-Progress — tasks currently being worked on.

---

### Q4. What is Lead Time?

**Answer:**
Time from request to completion.

---

### Q5. What is Throughput?

**Answer:**
Number of tasks completed in a given period.

---

# 🚀 One-Line Summary

> **Kanban helps teams visualize work, limit work in progress, and optimize workflow for continuous delivery.**
