# Phases of Software Engineering

> Beginner-friendly notes on Requirement Analysis, SRS, ERD, Software Design, and Coding.

---

# Table of Contents

1. Requirement Analysis
2. Software Requirement Specification (SRS)
3. Entity Relationship Diagram (ERD)
4. Software Design
5. High Level Design (HLD)
6. Low Level Design (LLD)
7. Construction Phase (Coding + Unit Testing)
8. Verification vs Validation
9. Quick Revision Notes
10. Interview Questions

---

# 1. Requirement Analysis

## Definition

Requirement Analysis is:
> The process of studying customer requirements carefully and removing ambiguities.

---

## Activities in Requirement Analysis

- Requirement Gathering
- Requirement Validation
- Stakeholder Discussions
- Documentation
- Identifying Missing Information

---

## Requirement Gathering Techniques

| Technique | Description |
|---|---|
| Interviews | Direct interaction with users |
| Surveys | Collecting feedback using forms |
| Observation | Studying existing systems |
| Workshops | Group discussions |
| Brainstorming | Generating ideas |

---

## Problems in Requirement Analysis

| Problem | Description |
|---|---|
| Ambiguous Requirements | Requirements are unclear |
| Incomplete Requirements | Missing information |
| Contradicting Requirements | Requirements conflict with each other |
| Changing Requirements | Requirements change frequently |

---

## Functional Requirements

Functional requirements describe:
> What the system should do.

### Examples
- User Login
- Generate Bill
- Online Payment
- Add Product

---

## Non-Functional Requirements

Non-functional requirements describe:
> How the system should perform.

### Examples
- Performance
- Security
- Reliability
- Portability

---

## Real-Time Example

### Functional Requirement
```text
ATM should allow cash withdrawal.
```

### Non-Functional Requirement
```text
ATM transaction should complete within 5 seconds.
```

---

# 2. Software Requirement Specification (SRS)

## Definition

SRS stands for:
```text
Software Requirement Specification
```

It is a document that describes:
- Functional Requirements
- Non-Functional Requirements
- Constraints
- User Expectations

---

## Purpose of SRS

- Helps developers understand requirements
- Helps testers prepare test cases
- Reduces confusion
- Acts as a contract between client and developers

---

## Properties of a Good SRS

| Property | Meaning |
|---|---|
| Concise | Short and clear |
| Complete | All requirements included |
| Consistent | No conflicting requirements |
| Verifiable | Requirements can be tested |
| Easy to Modify | Easy to update later |

---

## Constraints in SRS

| Constraint | Description |
|---|---|
| Hardware Constraint | Required hardware |
| OS Constraint | Supported operating system |
| DBMS Constraint | Database requirement |
| Standard Compliance | Industry standards |

---

# 3. Entity Relationship Diagram (ERD)

## Definition

ERD is:
> A visual representation of entities, attributes, and relationships in a database system.

---

## ERD Components

| Symbol | Meaning |
|---|---|
| Rectangle | Entity |
| Diamond | Relationship |
| Oval | Attribute |

---

## Cardinality Types

| Type | Meaning |
|---|---|
| 1:1 | One-to-One |
| 1:M | One-to-Many |
| M:M | Many-to-Many |

---

## Real-Time Examples

### One-to-One
```text
Person → Passport
```

### One-to-Many
```text
Department → Employees
```

### Many-to-Many
```text
Products ↔ Sales
```

---

# 4. Software Design

## Definition

Software Design converts:
```text
Requirements → System Specifications
```

---

## Objectives of Design

- Define architecture
- Define modules
- Prepare database structures
- Prepare for coding

---

## Importance of Design

| Benefit | Description |
|---|---|
| Better Planning | Clear structure |
| Reusability | Modules reused |
| Maintainability | Easier updates |
| Portability | Works on multiple platforms |

---

## Characteristics of Good Design

| Characteristic | Meaning |
|---|---|
| Efficiency | Better performance |
| Reliability | Accurate results |
| Flexibility | Easy modification |
| Portability | Works on multiple systems |
| Maintainability | Easy maintenance |

---

# 5. High Level Design (HLD)

## Definition

HLD provides:
> The overall architecture of the system.

---

## HLD Focuses On

- Modules
- System Architecture
- Database Design
- Module Communication

---

## Components of HLD

| Component | Description |
|---|---|
| Data Design | Database structure |
| Architectural Design | System architecture |
| Interface Design | User interaction |

---

## Real-Time Example

### Online Shopping System Modules
- User Module
- Product Module
- Payment Module
- Order Module

---

# 6. Low Level Design (LLD)

## Definition

LLD provides:
> Detailed logic and implementation details for modules.

---

## LLD Includes

- Algorithms
- Pseudocode
- Function Logic
- Data Structures

---

## Example Pseudocode

```text
Start

Read username
Read password

If valid
    Display "Login Successful"
Else
    Display "Invalid Credentials"

Stop
```

---

# Difference Between HLD and LLD

| HLD | LLD |
|---|---|
| Overall system design | Detailed module logic |
| Architecture focused | Algorithm focused |
| Module communication | Function implementation |

---

# 7. Construction Phase (Coding + Unit Testing)

## Definition

Construction Phase converts:
```text
Design → Working Software
```

---

## Activities

| Activity | Description |
|---|---|
| Coding | Writing source code |
| Unit Testing | Testing modules |
| Database Creation | Creating databases |

---

## Outputs

- Source Code
- Executable Files
- Databases

---

# Unit Testing

## Definition

Unit Testing checks:
> Individual modules independently.

---

## Advantages

- Finds bugs early
- Improves code quality
- Simplifies debugging
- Reduces maintenance cost

---

# Construction Guidelines

- Use proper coding standards
- Use meaningful variable names
- Maintain proper indentation
- Perform reviews and testing
- Apply Verification & Validation

---

# 8. Verification vs Validation

| Verification | Validation |
|---|---|
| Build product correctly | Build correct product |
| Process-oriented | Product-oriented |
| During development | After development |

---

# 9. Quick Revision Notes

| Topic | Key Point |
|---|---|
| Requirement Analysis | Study customer requirements |
| SRS | Requirement document |
| ERD | Database design diagram |
| HLD | Overall architecture |
| LLD | Detailed logic |
| Functional Requirement | What system does |
| Non-Functional Requirement | How system performs |
| Unit Testing | Tests individual modules |

---

# 10. Important Interview Questions

## Q1. What is Requirement Analysis?
Requirement Analysis is the process of studying and validating customer requirements.

---

## Q2. What is SRS?
SRS is a document that specifies software requirements clearly.

---

## Q3. Difference between Functional and Non-Functional Requirements?

| Functional | Non-Functional |
|---|---|
| What system does | How system performs |

---

## Q4. What is HLD?
HLD describes the overall system architecture and modules.

---

## Q5. What is LLD?
LLD describes detailed algorithms and module logic.

---

## Q6. What is ERD?
ERD is used to represent entities and relationships in databases.

---

## Q7. What is Unit Testing?
Unit Testing tests individual modules independently.

---

# Conclusion

These Software Engineering phases help developers:
- Understand requirements clearly
- Design software properly
- Build reliable applications
- Improve software quality
- Reduce development errors
