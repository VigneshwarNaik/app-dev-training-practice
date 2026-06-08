# Phases of Software Engineering 

## Introduction

Software Engineering is a systematic process used to develop high-quality software. It consists of several phases that help developers understand requirements, design the system, build the software, test it, and maintain it after deployment.

---

## 1. Requirement Analysis

### Definition

Requirement Analysis is the process of understanding and collecting customer requirements.

### Bank App Example

The bank wants:

* User Login
* Check Balance
* Money Transfer

### Output

A clear list of requirements.

### Simple Meaning

Talk to the customer and understand what they need.

---

## 2. Software Requirement Specification (SRS)

### Definition

SRS (Software Requirement Specification) is a document that contains all software requirements.

### Example

#### Functional Requirements

* Login
* Balance Inquiry
* Money Transfer

#### Non-Functional Requirements

* Security
* Fast Response
* 24/7 Availability

### Output

SRS Document

### Simple Meaning

Write all requirements clearly in one document.

---

## 3. Entity Relationship Diagram (ERD)

### Definition

ERD is a visual representation of database entities and their relationships.

### Example

```text
Customer
   |
   |
 Account
   |
   |
Transaction
```

### Output

Database Structure

### Simple Meaning

Design how data will be stored in the database.

---

## 4. High Level Design (HLD)

### Definition

HLD describes the overall architecture of the system.

### Example

```text
Bank App
│
├── Login Module
├── Account Module
├── Transfer Module
└── Payment Module
```

### Output

System Architecture

### Simple Meaning

Create the big picture of the application.

---

## 5. Low Level Design (LLD)

### Definition

LLD describes detailed logic and implementation of each module.

### Example

```text
Start
Read Username
Read Password

If Correct
    Login Success
Else
    Login Failed

Stop
```

### Output

Algorithms and Pseudocode

### Simple Meaning

Design detailed steps for each feature.

---

## 6. Coding

### Definition

Coding converts design into a working software application.

### Example

```java
if(username.equals("admin")) {
    System.out.println("Login Success");
}
```

### Output

Source Code

### Simple Meaning

Write program code.

---

## 7. Unit Testing

### Definition

Unit Testing tests each module independently.

### Example

Login Module Testing:

* Correct Password ✅
* Wrong Password ✅

### Output

Bug-Free Modules

### Simple Meaning

Test each small part separately.

---

## 8. Verification

### Definition

Verification checks whether the software is being developed correctly.

### Example

* Did developers follow the design?
* Is login implemented correctly?

### Simple Meaning

Build the product correctly.

---

## 9. Validation

### Definition

Validation checks whether the software meets customer requirements.

### Example

The bank requested money transfer functionality. Does the app provide it?

### Simple Meaning

Build the correct product.

---

## 10. Deployment

### Definition

Deployment releases the software to end users.

### Example

Publish the bank app on Android and iOS.

### Output

Working Software for Users

### Simple Meaning

Launch the software.

---

## 11. Maintenance

### Definition

Maintenance involves fixing bugs and adding improvements after deployment.

### Example

After six months:

* Add UPI Payments
* Add Bill Payments
* Fix Bugs

### Output

Updated Software

### Simple Meaning

Support and improve the software after release.

---

# Complete Flow

```text
Requirement Analysis
        ↓
SRS
        ↓
ERD
        ↓
HLD
        ↓
LLD
        ↓
Coding
        ↓
Unit Testing
        ↓
Verification
        ↓
Validation
        ↓
Deployment
        ↓
Maintenance
```

# Quick Revision

| Phase                | Purpose                     |
| -------------------- | --------------------------- |
| Requirement Analysis | Understand customer needs   |
| SRS                  | Document requirements       |
| ERD                  | Design database             |
| HLD                  | Design overall architecture |
| LLD                  | Design detailed logic       |
| Coding               | Write source code           |
| Unit Testing         | Test individual modules     |
| Verification         | Build product correctly     |
| Validation           | Build correct product       |
| Deployment           | Release software            |
| Maintenance          | Fix and improve software    |

## Conclusion

Software Engineering follows a structured approach to develop reliable software. The phases include Requirement Analysis, SRS, ERD, HLD, LLD, Coding, Testing, Verification, Validation, Deployment, and Maintenance. Following these phases helps reduce errors and improve software quality.
