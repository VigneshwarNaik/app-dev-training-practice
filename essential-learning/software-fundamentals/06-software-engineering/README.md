# Software Engineering (SE) Notes

# 📘 Introduction

Software Engineering is a systematic and disciplined approach used for developing high-quality software.

Software development follows a structured process called the:

> Software Development Life Cycle (SDLC)

SDLC helps in:
- Requirement gathering
- Planning
- Designing
- Coding
- Testing
- Deployment
- Maintenance

---
# SDLC (Software Development Life Cycle)

## 📌 Overview

SDLC (Software Development Life Cycle) is a structured process used to develop high-quality software. It helps teams plan, design, build, test, deploy, and maintain software efficiently.

---

## 🔄 Phases of SDLC

### 1. Requirement Gathering 📋

In this phase, the development team collects and understands the client's requirements.

#### Example

A restaurant owner wants a Food Delivery App with:

* User Registration
* Food Ordering
* Online Payment
* Order Tracking

#### Output

Requirement Specification Document (SRS)

---

### 2. Planning 📅

The project team estimates:

* Cost
* Time
* Resources
* Team Members

#### Example

* 3 Developers
* 2 Testers
* 1 UI Designer
* Project Duration: 4 Months

#### Output

Project Plan

---

### 3. Designing 🎨

Designers create:

* User Interface (UI)
* Database Design
* System Architecture

#### Example Flow

```text
Login
  ↓
Restaurant List
  ↓
Food Menu
  ↓
Cart
  ↓
Payment
```

#### Output

Design Documents and Wireframes

---

### 4. Coding 💻

Developers write the source code based on the design.

#### Example

Modules Developed:

* Login Module
* Food Ordering Module
* Payment Module
* Order Tracking Module

#### Output

Working Software Application

---

### 5. Testing 🧪

Testers verify that the software works correctly and identify bugs.

#### Example

**Test Case 1**

```text
Input: Add Pizza to Cart
Action: Place Order
Expected Result: Order Successfully Placed
```

**Test Case 2**

```text
Input: Incorrect Password
Expected Result: Error Message Displayed
```

#### Output

Bug Reports and Tested Application

---

### 6. Deployment 🚀

The application is released to end users.

#### Example

Food Delivery App is deployed to:

* Google Play Store
* Apple App Store

#### Output

Live Application

---

### 7. Maintenance 🔧

After deployment, bugs are fixed and new features are added.

#### Example

* Fix payment crash issue
* Add UPI payment option
* Improve app performance

#### Output

Updated Application

---

## 📊 SDLC Flow

```text
Requirement Gathering
          ↓
      Planning
          ↓
      Designing
          ↓
       Coding
          ↓
      Testing
          ↓
     Deployment
          ↓
     Maintenance
```

---

## 🎯 Advantages of SDLC

* Improves software quality
* Reduces development risks
* Ensures proper planning
* Helps deliver projects on time
* Simplifies maintenance and updates

---

## 📝 Conclusion

SDLC provides a systematic approach for software development. By following its phases—Requirement Gathering, Planning, Designing, Coding, Testing, Deployment, and Maintenance—organizations can build reliable, efficient, and high-quality software products.





# 📑 Table of Contents

- Introduction
- SDLC Models
  - Prototype Model
  - RAD Model
  - Incremental Model
  - Spiral Model
- Comparison Table
- Conclusion
- Key Takeaways

---

# 🎯 Objectives

After completing this module, you will be able to:

- Understand SDLC concepts
- Explain different SDLC models
- Understand Prototype Model
- Explain RAD Model
- Explain Incremental Model
- Explain Spiral Model
- Understand advantages and limitations of each model

---

# 📚 Traditional SDLC Models

The major SDLC models are:

1. Waterfall Model
2. V-Model
3. Prototype Model
4. RAD Model
5. Incremental Model
6. Spiral Model

---

# 1️⃣ Prototype Model

# 📖 Definition

Prototype Model is the process of developing a sample or incomplete version of software before developing the final product.

It helps developers and clients:
- Understand requirements
- Clarify doubts
- Improve communication
- Reduce development risks

---

# ✨ Features of Prototype Model

- Creates an incomplete version of software
- Simulates only important features
- User feedback is collected continuously
- Requirements become clearer gradually

---

# 🔄 Steps in Prototype Model

1. Identify basic requirements
2. Develop initial prototype
3. Review by users
4. Refine the prototype
5. Repeat until client satisfaction
6. Develop final software

---

# 📌 Prototype Development Process

```text
Requirements
      ↓
Quick Design
      ↓
Build Prototype
      ↓
User Evaluation
      ↓
Refining Prototype
      ↓
Implementation & Maintenance
```

---

# 🎯 Why Prototype Model is Used

Prototype Model is useful because:

- Helps software architects make decisions
- Improves communication among team members
- Helps test ideas quickly
- Allows users to suggest additional requirements
- Provides early feedback

---

# 🧩 Types of Prototype Model

## 1. Throwaway Prototype Model

### Throwaway Prototype Model (Software Engineering)

**Definition:**
The Throwaway Prototype Model is a software development model in which a **temporary prototype** is created to understand and clarify user requirements. After gathering feedback, the prototype is **discarded (thrown away)**, and the actual system is developed from scratch.

### Steps:

1. Gather initial requirements.
2. Build a quick prototype.
3. Show the prototype to the customer.
4. Collect feedback and refine requirements.
5. Discard the prototype.
6. Develop the final system based on the confirmed requirements.

### Real-Time Example:

Suppose a bank wants a new mobile banking app.

* Developers first create a simple prototype showing login, account balance, and money transfer screens.
* The bank reviews it and suggests changes.
* Once requirements are finalized, the prototype is discarded.
* The actual banking application is then developed properly.

### Advantages:

* Helps understand user requirements clearly.
* Reduces requirement misunderstandings.
* Improves customer involvement.
* Saves cost by finding issues early.

### Disadvantages:

* Extra time and effort spent on building a prototype.
* Users may think the prototype is the final product.
* The prototype itself cannot be reused.

### Diagram:

```text
Requirements
      ↓
Quick Design
      ↓
Prototype
      ↓
Customer Evaluation
      ↓
Refined Requirements
      ↓
Discard Prototype
      ↓
Develop Final System
```


## 2. Evolutionary Prototype Model

Evolutionary Prototype Model
Definition

The Evolutionary Prototype Model is a software development model in which a prototype is built first and then continuously improved and refined based on user feedback until it becomes the final software product.

Unlike the Throwaway Prototype Model, the prototype is not discarded. It evolves into the final system.

Steps
Gather basic requirements.
Develop an initial prototype.
Show it to the customer.
Collect feedback.
Modify and improve the prototype.
Repeat the process until the final system is ready.

Real-Time Example

Suppose a company wants an Online Shopping Application.

First, developers create a simple prototype with login and product display features.
Users test it and request a shopping cart feature.
Developers add the cart feature.
Users request online payment and order tracking.
These features are added gradually.
The prototype keeps evolving until it becomes the complete shopping application.
Advantages
Better understanding of user requirements.
Continuous customer involvement.
Changes can be made easily.
Faster delivery of a working system.
Disadvantages
Development cost may increase.
Project scope may keep changing.
Requires frequent user feedback.
Diagram
Basic Requirements
        ↓
Initial Prototype
        ↓
Customer Evaluation
        ↓
Feedback
        ↓
Refine Prototype
        ↓
Customer Evaluation
        ↓
Refine Again
        ↓
Final System



# ✅ Advantages of Prototype Model

1. Reduced development time and cost
2. Active user involvement
3. Early visibility of product
4. Improved software quality
5. Better understanding of requirements
6. Continuous feedback from users

---

# ❌ Limitations of Prototype Model

1. Frequent requirement changes
2. Increased complexity
3. Documentation may become weak
4. Additional management effort required
5. Users may expect the final product too early

---

# 📌 When to Use Prototype Model

Prototype Model is suitable when:

- Requirements are unclear
- User interaction is high
- Frequent feedback is required
- System design is complex

---

# 2️⃣ Rapid Application Development (RAD) Model

# Rapid Application Development (RAD) Model

### Definition

The **Rapid Application Development (RAD) Model** is a software development model that focuses on **quick development and fast delivery** of software by using reusable components, prototyping, and continuous user feedback.

 The Rapid Application Development (RAD) Model is a software development model that emphasizes rapid prototyping, reusable components, and continuous user feedback to develop and deliver software quickly.


The main goal is to develop the software in a short time.

---

### Phases of RAD Model

1. **Requirements Planning**

   * Gather user requirements.

2. **User Design**

   * Create prototypes and get user feedback.

3. **Construction**

   * Develop the actual application quickly using reusable components.

4. **Cutover**

   * Testing, deployment, and maintenance.

---

### Bank Mobile App Example

#### Requirement Planning

A bank wants a mobile banking application with:

* Login
* Balance Inquiry
* Money Transfer
* Transaction History

#### User Design

Developers quickly create screens for:

* Login Page
* Account Dashboard
* Money Transfer Page

The bank reviews the screens and suggests changes.

#### Construction

Developers rapidly build the application using existing components and frameworks.

Features added:

* Login
* Balance Check
* Fund Transfer
* Transaction History
* UPI Payments

#### Cutover

* Test the application
* Fix bugs
* Deploy to users

---

### Diagram

```text
Requirements Planning
          ↓
      User Design
          ↓
     Construction
          ↓
       Cutover
          ↓
     Final System
```

---

### Advantages

* Faster development.
* Reduced development time.
* Continuous customer involvement.
* Easy to accommodate changes.

### Disadvantages

* Requires skilled developers.
* Not suitable for very large projects.
* Depends heavily on customer feedback.

---

### Real-Time Example

A bank needs a mobile banking app within 3 months. Instead of developing everything from scratch, developers use ready-made components for login, payment processing, and notifications. The app is developed quickly, tested, and delivered in a short time.

---

# 3️⃣ Incremental Model

Definition

The Incremental Model is a software development model in which the software is developed and delivered in small parts (increments). Each increment adds new features to the system until the complete product is finished.

Bank Mobile App Example

Suppose a bank wants a mobile banking application.

Increment 1

Develop basic features:

Login
Account Balance
Login → View Balance

The bank starts using this version.

Increment 2

Add:

Money Transfer
Login
  ↓
View Balance
  ↓
Transfer Money
Increment 3

Add:

Transaction History
Login
  ↓
View Balance
  ↓
Transfer Money
  ↓
Transaction History
Increment 4

Add:

UPI Payments
Bill Payments
Bank Mobile App
│
├── Login
├── Balance Inquiry
├── Money Transfer
├── Transaction History
├── UPI Payments
└── Bill Payments

Now the complete banking application is ready.

Phases

For each increment:

Requirements Analysis
Design
Coding
Testing
Deployment
Diagram
Increment 1 → Basic Features
        ↓
Increment 2 → More Features
        ↓
Increment 3 → More Features
        ↓
Increment 4 → Complete System
Advantages
Working software is delivered early.
Easy to test and debug.
Customer can use features sooner.
Changes can be made between increments.
Disadvantages
Requires proper planning.
Integration of increments can be difficult.
Overall cost may increase.
Real-Time Example

A bank first releases a mobile app with Login and Balance Inquiry. Later updates add Money Transfer, Transaction History, and UPI Payments. The application grows feature by feature until it becomes a complete banking app.


# 4️⃣ Spiral Model

# Spiral Model

### Definition

The **Spiral Model** is a software development model that combines features of the **Waterfall Model** and **Prototyping Model**. It focuses heavily on **risk analysis**. Development is done in repeated cycles called **spirals**.

Each spiral includes:

1. Planning
2. Risk Analysis
3. Development
4. Customer Evaluation

---

### Bank Mobile App Example

Suppose a bank wants a mobile banking app.

### First Spiral

**Planning**

* Need Login and Balance Inquiry.

**Risk Analysis**

* Can user data be kept secure?

**Development**

* Create Login and Balance features.

**Evaluation**

* Bank reviews the system.

---

### Second Spiral

**Planning**

* Add Money Transfer.

**Risk Analysis**

* Risk of incorrect transactions or fraud.

**Development**

* Implement Money Transfer.

**Evaluation**

* Bank tests and provides feedback.

---

### Third Spiral

**Planning**

* Add UPI Payments.

**Risk Analysis**

* Payment security and server load risks.

**Development**

* Implement UPI feature.

**Evaluation**

* Customer feedback and testing.

---

### Diagram

```text
Spiral 1
(Plan → Risk → Develop → Evaluate)
                ↓
Spiral 2
(Plan → Risk → Develop → Evaluate)
                ↓
Spiral 3
(Plan → Risk → Develop → Evaluate)
                ↓
Final System
```

---

### Real-Time Example

When a bank develops a mobile banking app, security risks are very important. Before adding each feature (Login, Money Transfer, UPI), developers analyze possible risks, solve them, develop the feature, and then get customer feedback. This cycle continues until the complete app is ready.

---

### Advantages

* Excellent risk management.
* Suitable for large and complex projects.
* Customer feedback is included in every cycle.
* Changes can be handled easily.

### Disadvantages

* Costly and time-consuming.
* Requires risk analysis experts.
* Not suitable for small projects.

---

> The Spiral Model is a software development model in which the project is developed through repeated cycles called spirals. Each spiral includes planning, risk analysis, development, and customer evaluation, with a strong focus on risk management.

### Easy Way to Remember

**Incremental Model:**
"Add feature → Deploy → Add another feature → Deploy"

**Spiral Model:**
"Plan → Check Risks → Develop → Get Feedback → Repeat"

The main difference is that **Spiral Model focuses on risk analysis before every development cycle**.


---


# 📊 Comparison of Models

| Model | Best For | Flexibility | Risk Handling | Customer Feedback |
|---|---|---|---|---|
| Prototype | Unclear requirements | High | Medium | High |
| RAD | Fast development | High | Medium | High |
| Incremental | Large modular systems | Medium | Medium | Medium |
| Spiral | High-risk projects | High | High | High |

---

# 🎯 Final Conclusion

Different SDLC models are selected based on:

- Project size
- Requirement clarity
- Risk level
- Budget
- Time constraints

## Quick Summary

| Model | Main Purpose |
|---|---|
| Prototype | Clarify requirements |
| RAD | Fast development |
| Incremental | Gradual software delivery |
| Spiral | Risk management |

Choosing the correct SDLC model improves:
- Software quality
- Customer satisfaction
- Development efficiency
- Project success

---

# 📚 Key Takeaways

- SDLC provides a structured software development process
- Prototype Model helps understand unclear requirements
- RAD focuses on rapid software development
- Incremental Model develops software step-by-step
- Spiral Model focuses heavily on risk analysis
- Every SDLC model has advantages and limitations
