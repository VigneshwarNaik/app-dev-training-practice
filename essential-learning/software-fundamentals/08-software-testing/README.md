# Software Testing Introduction

## ✈️ Flight Safety and Software Testing

Have you ever wondered about the precautions the pilot and his crew have to take before a flight is prepared for takeoff?

In the flight testing process, many aspects of the aircraft must be checked carefully:

- Engines
- Vertical and horizontal stabilizers
- Rudder
- Ailerons
- Fuselage
- Cockpit controls
- Measuring dials and panels
- Parachutes
- Seats
- Life jackets
- Oxygen masks

And many other important parts too.

Imagine if these checks were not done properly. Even a small mistake could create serious problems during the flight.

Because safety is extremely important, many of these checks are repeated several times by different teams to ensure everything works correctly without failure.

A safe and happy flight depends on proper testing.

---

# 💻 Software Testing

Just like aircraft testing, software testing is also an important phase in developing a software product.

There has been a history of major software failures only because:

- Testing was overlooked
- Testing was not done properly
- Errors were discovered too late

Software testing helps in:

- Finding bugs and errors
- Improving software quality
- Ensuring reliability
- Providing a better user experience
- Preventing software failures

---

# 📌 Importance of Testing

Testing is important and needs to be done as early as possible in every phase of the Software Development Life Cycle (SDLC), and even after the software product is developed.

Proper testing ensures:

✅ Better software quality  
✅ Reduced risk of failure  
✅ Improved performance  
✅ Increased customer satisfaction  
✅ Safe and reliable applications  

---

# 🎯 Conclusion

Software testing plays a crucial role in software development.  
Just like flight safety checks protect passengers, software testing protects users from software failures and ensures the software works correctly and efficiently.



# 🧪 Software Testing Notes

# 📌 Objectives

After completing this module, you will be able to:

- Explain testing concepts
- Understand the importance of testing
- Elaborate Software Testing Life Cycle (STLC) phases
- Identify the levels of testing

---

# ✈️ Introduction to Testing

Software testing is similar to aircraft safety testing.

Before a flight takes off, many parts are checked:

- Engines
- Stabilizers
- Rudder
- Cockpit controls
- Oxygen masks
- Safety equipment

These checks are repeated multiple times to ensure safety.

Similarly, software testing ensures that the software works correctly, safely, and efficiently before it is released to users.

---

# 🧠 Scenario 1 – OMR Evaluation

An organization conducted a hiring test using OMR sheets.

The software checks whether the candidate shaded the correct option.

### Problem

If a candidate shades **all options for every question**, the system may still give full marks because the correct option is included.

### Learning

Testing should focus on:

- Finding defects
- Identifying faults
- Detecting unexpected behavior

A good tester tries to find errors instead of proving that the software is always correct.

---

# 🏦 Scenario 2 – Banking Application

A banking application was tested with valid and invalid inputs.

Everything worked correctly.

### Problem

After logout, the client clicked the **Back button** and could still access previous pages and perform transactions.

### Learning

This is a major security flaw.

Testing must also check:

- Security
- Session handling
- Unexpected user actions

---

# 🧪 Definition of Software Testing

Software testing is the process of executing a program with the intention of finding errors.

## Verification and Validation (V&V)

### Verification
**"Are we building the product right?"**

Checks whether development follows specifications correctly.

### Validation
**"Are we building the right product?"**

Checks whether the product satisfies user needs.

---

# ✅ IEEE 610 Standard Definition

Software Testing is the process of exercising or evaluating a system manually or automatically to verify that it satisfies specified requirements or to identify differences between actual and expected results.

---

# 🎯 Importance and Need of Testing

Software testing is important because it:

- Ensures the software meets requirements
- Saves money by identifying defects early
- Reduces risks in software
- Improves trust and reliability
- Helps communicate software limitations to users

## Example

In a university student management system:

- Incorrect marks displayed due to a bug is a software failure.
- Proper testing could instead display:
  
  `"Unable to display marks. Please try later."`

Early testing prevents errors from affecting later stages.

---

# 🐞 Debugging

Debugging is the process of finding the source of identified bugs and fixing them.

## Performed By
Developers

## Steps in Debugging

1. Find the defect in the code
2. Identify the root cause
3. Locate the exact problem area
4. Fix the defect
5. Recheck to ensure everything works correctly

---

# 🔄 Software Testing Life Cycle (STLC)

STLC identifies testing activities and determines the best time to perform them.

## Phases of STLC

### 1. Test Planning
- Resource allocation
- Creating test environment
- Test scheduling

### 2. Test Design
- Writing test scenarios
- Preparing test cases
- Creating test data and scripts

### 3. Test Execution
- Executing test scripts
- Finding bugs

### 4. Reporting to Developers
- Reporting defects
- Regression testing after bug fixes

### 5. Test Cycle Closure
- Documentation of testing activities
- Final reports preparation

---

# ⚙️ Methodologies of Testing

## Manual Testing

Testing performed manually by QA testers.

## Automated Testing

Uses automation tools and scripts to compare expected and actual results.

### Examples
- JUnit (Java)
- NUnit (.NET)

## Defect Tracking

Process of logging and monitoring bugs during testing.

### Example Tools
- Bugzilla

---

# 🧩 Unit Testing

## Done By
Developers

## Purpose

- Tests individual modules
- Verifies whether modules meet specifications
- Validates code written during development

## Who Performs It?

- Software developers
- Sometimes independent testers

---

# 🔗 Integration Testing

## Done By
Developers or Independent Testers

## Definition

Integration testing checks whether combined modules work correctly together.

## Purpose

To expose faults in the interaction between integrated units.

---

# 🖥️ System Testing

## Performed By
Testers

## Aim

Find differences between implementation and specification.

## Types

### Functional Testing
Tests whether business requirements are implemented correctly.

### Performance Testing
Tests non-functional requirements like speed and stability.

---

# 🔼 Top-Down Testing

- Top-level modules are tested first
- Lower modules are tested later
- Uses **Stubs** to simulate lower-level modules

## Stub
A dummy module used for called functions.

---

# 🔽 Bottom-Up Testing

- Bottom-level modules are tested first
- Higher modules are tested later
- Uses **Drivers** to simulate higher-level modules

## Driver
A dummy module used to call other modules.

---

# 🚀 Performance Testing Types

## Stress Testing
Evaluates the system under extreme conditions.

## Regression Testing
Ensures changes or bug fixes do not affect existing functionality.

## Usability Testing
Checks user-friendliness and ease of use.

---

# 👤 User Acceptance Testing (UAT)

## Done By
Client or End Users

## Objective

To confirm that the system satisfies user requirements and is ready for delivery.

## Types of UAT

### Alpha Testing
Performed by the client in the developer’s environment.

### Beta Testing
Performed by the client in the real-world environment.

---

# 📚 Conclusion

Software testing is a critical process in software development.

It helps to:

- Detect defects early
- Improve software quality
- Ensure security and reliability
- Deliver a better user experience

Testing ensures that software works correctly before reaching users.


# 🧪 Testing Principles and Static Testing Notes

# 📌 Objectives

After completing this module, you will be able to:

- Explain testing principles
- Identify the two types of testing
- Understand the concepts of static testing
- Elaborate Review, Walkthrough, and Inspection

---

# 🧠 Testing Principles

Software testing follows seven important principles that help ensure effective testing.

## Seven Testing Principles

1. Testing shows the presence of defects  
2. Early testing  
3. Exhaustive testing is impossible  
4. Defect clustering  
5. Pesticide paradox  
6. Testing is context dependent  
7. Absence of error fallacy  

---

# 📖 Explanation of Testing Principles

## 1️⃣ Testing Shows the Presence of Defects

Testing can show that defects exist in the software, but it cannot prove that the software is completely error-free.

---

## 2️⃣ Early Testing

Testing should begin early in every phase of the Software Development Life Cycle (SDLC).

### Benefits
- Defects are found early
- Cost of fixing bugs is reduced
- Improves software quality

---

## 3️⃣ Exhaustive Testing is Impossible

Testing all possible inputs, combinations, and conditions is not practical.

### Therefore:
- Test cases are selected carefully
- Risk-based testing is used

---

## 4️⃣ Defect Clustering

A small number of modules usually contain most of the defects.

### Meaning
Some parts of the software are more error-prone than others.

---

## 5️⃣ Pesticide Paradox

Repeating the same test cases again and again may not find new defects.

### Solution
- Revise test cases regularly
- Create new test cases
- Test different parts of the application

---

## 6️⃣ Testing is Context Dependent

Testing methods differ based on the type of application.

### Example
- Testing a banking system is different from testing a library management system.
- Mission-critical systems require stricter testing.

---

## 7️⃣ Absence of Error Fallacy

Even if no defects are found, the software may still fail if it does not meet user requirements.

### Meaning
Bug-free software is useless if it does not satisfy customer needs.

---

# 🔄 Types of Testing

Software testing is mainly divided into two types:

## 1️⃣ Static Testing

### Techniques
- Review
- Walkthrough
- Inspection

---

## 2️⃣ Dynamic Testing

### Techniques
- Black Box Testing
- White Box Testing

---

# 📄 Static Testing

Static testing checks software work products manually without executing the code.

## Features of Static Testing

### 📝 Manual Process
Testing is done manually to identify errors.

### 📚 Work Products
Includes:
- Documents
- Requirements
- Design files
- Source code

### 🛠️ Techniques Used
- Reviews
- Walkthroughs
- Inspections

### 🚫 No Code Execution
The program is not executed during static testing.

Static testing checks:
- Code quality
- Standards
- Documentation
- Logic errors

---

# 👥 Members of Static Testing

Different people participate in static testing activities.

## Members

### 👨‍💻 Author
Person who created the document or code.

### 👨‍🏫 Moderator
Leads and controls the review process.

### 📖 Reader
Reads and explains the work product.

### 📝 Recorder / Scribe
Records findings and defects.

### 🔍 Inspector
Examines the product carefully for defects.

---

# 🛠️ Techniques in Static Testing

## 1️⃣ Review

Review is the process in which a product is re-examined or re-evaluated to identify corrections or improvements.

---

## 2️⃣ Walkthrough

Walkthrough is mostly performed on developed code.

### Process
- The author explains the code
- Sample test data is used
- Intermediate results are recorded

---

## 3️⃣ Inspection

Inspection is a formal review technique.

### Features
- Step-by-step examination
- Compared against predefined criteria
- Uses standards and historical defect lists

---

# 🔍 Review Process

Review is a static testing technique where artifacts are manually examined.

## Artifacts Reviewed

- SRS documents
- Design specifications
- Source code
- Test plans
- Test specifications
- Test cases
- Test scripts
- User guides
- Web pages

---

# 🔄 Steps in Review Process

1. Planning  
2. Identifying entry and exit criteria  
3. Initiating review  
4. Verifying entry criteria  
5. Self preparation  
6. Marking questions and comments  
7. Recording results  
8. Rework  
9. Defect fixing if needed  
10. Follow up  
11. Verifying exit criteria  

---

# 🚶 Walkthrough

Walkthrough is a review meeting led by the author.

## Features of Walkthrough

- Focuses on dry runs of code and scenarios
- Can begin informally and become formal
- Peer groups participate
- Main goal is finding defects
- Review reports are prepared

---

# 🔎 Inspection

Inspection is a formal static testing method.

## Features of Inspection

- Prepared before the meeting
- Led by a trained moderator
- Focuses on defect detection
- Uses entry and exit criteria
- Inspection reports contain findings
- Follow-up process is formal

---

# ✅ Advantages of Static Testing

Static testing provides several benefits.

## Advantages

- Early defect detection and correction
- Fewer defects in software
- Improves development productivity
- Helps identify missing requirements
- Saves testing cost and time
- Improves communication within the team

---

# 📚 Conclusion

Testing principles help testers follow the right testing strategy.

Static testing helps detect defects early without executing the program, saving time, cost, and effort in software development.

Techniques like:
- Reviews
- Walkthroughs
- Inspections

play an important role in improving software quality before execution begins.

# Dynamic Testing – Software Testing Notes

## Objectives

After completing this module, you will be able to:

- Explain the concept of Dynamic Testing
- Describe Black Box Testing and White Box Testing

---

# Types of Testing

There are two types of testing:

## 1. Static Testing
Testing done without executing the program.

### Techniques:
- Review
- Walkthrough
- Inspection

---

## 2. Dynamic Testing
Testing done by executing the software.

### Techniques:
- Black Box Testing
- White Box Testing

---

# Dynamic Testing – Black Box Testing

Black Box Testing tests the functionality of the software without knowing the internal code structure.

## Features
- Focuses on inputs and outputs
- Internal code is ignored
- Finds defects through testing behavior

## Example
Input → System → Output

If invalid input produces wrong output, defects are identified.

---

# Test Cases

A test case specifies:
- Input data
- Execution conditions
- Expected result
- Success criteria

## Purpose
- Verify whether requirements are working correctly
- Detect defects in the software

---

# Equivalence Class Partitioning (ECP)

A black-box testing technique.

## Definition
Input data is divided into groups called equivalence classes.

Each class behaves similarly, so one test case from each class is enough.

---

## Guidelines

For a range:
- One value below the range
- One value within the range
- One value above the range

---

## Example

Valid range = 1 to 1000

| Test Value | Type |
|---|---|
| 0 | Invalid |
| 500 | Valid |
| 1001 | Invalid |

---

# ECP Example Scenario

A grading system generates grades:

| Marks | Grade |
|---|---|
| >= 70 | A |
| 50 – 69 | B |
| 30 – 49 | C |
| < 30 | D |

If marks are outside the valid range, an error message is generated.

---

# Boundary Value Analysis (BVA)

A black-box testing technique focused on boundary values.

## Definition
Errors usually occur at boundaries rather than center values.

---

## Rule

If range is between `a` and `b`, test:
- a
- b
- just below a
- just above b

---

## Example

Range = 5 to 20

| Test Values |
|---|
| 4 |
| 5 |
| 20 |
| 21 |

---

# Cause Effect Analysis

Used to identify relationships between:
- Causes (inputs)
- Effects (outputs)

---

## Features

- Cause = Input condition
- Effect = Output condition
- Helps derive test cases
- Suitable when input combinations are few

---

# Cause Effect Example

Increment percentage depends on:
- Experience
- Designation

## Rules

| Experience | Increment |
|---|---|
| 1 – 3 years | 10% |
| 4 – 10 years | 20% |
| > 10 years | 30% |

---

# Cause Effect Graphing

Used to represent relationships between inputs and outputs.

## Steps
1. Identify causes and effects
2. Draw cause-effect graph
3. Convert graph into decision table
4. Generate test cases

---

## Logic Symbols

| Symbol | Meaning |
|---|---|
| NOT | Negation |
| OR | Either condition |
| AND | Both conditions |

---

# Decision Table Example

| C1 | C2 | C3 | A1 | A2 |
|---|---|---|---|---|
| 1 | 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 0 | 1 |
| 0 | 0 | 1 | 1 | 0 |

---

# State Transition Diagram

A black-box testing technique.

## Components

1. States  
2. Transitions  
3. Events  
4. Actions  

---

## Example

### States
- Open
- Closed

### Events
- Open file
- Close file

---

## Test Cases

| Initial State | Event | Output | Final State |
|---|---|---|---|
| Open | Close file | File closed | Closed |
| Closed | Open file | File opened | Open |
| Open | Open file | Invalid | Open |

---

# Ad-hoc Testing

An informal testing approach based on:
- Experience
- Intuition

## Example Test Cases
- Empty file
- File not available
- File with read permission

---

# Black Box Testing Scenario

Employee incentive based on appraisal rating.

| Rating | Incentive |
|---|---|
| 7 – 10 | 1000 USD |
| 4 – 6 | 500 USD |
| 1 – 3 | 300 USD |

---

## Test Data

### Equivalence Partitioning
- 3, 9, 12
- 2, 5, 9
- -2, 2, 5

### Boundary Value Analysis
- 6, 7, 10, 11
- 3, 4, 6, 7
- -1, 1, 3, 4

---

# Dynamic Testing – White Box Testing

Also called:
- Glass Box Testing
- Structural Testing
- Clear Box Testing

---

## Features

- Tests internal code structure
- Test cases derived from program structure
- Requires programming knowledge

---

## Tester Should Know
- Problem domain
- Internal implementation of code

---

# Basis Path Testing

A white-box testing method.

## Main Features

Design test cases to cover:
- Every statement
- Every condition
- Loops

---

# Statement Coverage

Checks whether every statement in the code is executed.

## Formula

```text
Statement Coverage =
(Number of statements executed / Total statements) × 100
```

---

# Branch Coverage

Measures decision coverage.

## Formula

```text
Branch Coverage =
(Number of branches covered / Total branches) × 100
```

---

# Loop Coverage

Checks how many times loops execute.

## Cases
- 0 times
- 1 time
- Multiple times

---

# Cyclomatic Complexity (McCabe’s Number)

Measures logical complexity of the program.

## Uses
- Finds number of independent paths
- Determines minimum test cases needed

---

## Steps

1. Break module into blocks
2. Create control flow graph
3. Connect nodes using arrows
4. Count regions

---

# Summary

## Black Box Testing
- Tests functionality
- No knowledge of code needed
- Techniques:
  - ECP
  - BVA
  - State Transition
  - Cause Effect Analysis

---

## White Box Testing
- Tests internal structure
- Requires coding knowledge
- Techniques:
  - Statement Coverage
  - Branch Coverage
  - Loop Coverage
  - Basis Path Testing

---

# Important Interview Questions

1. What is Dynamic Testing?
2. Difference between Black Box and White Box Testing?
3. What is Equivalence Class Partitioning?
4. Explain Boundary Value Analysis.
5. What is State Transition Testing?
6. Define Statement Coverage.
7. What is Loop Coverage?
8. Explain Cyclomatic Complexity.
9. What is Cause Effect Graphing?
10. What is Basis Path Testing?

---

# Conclusion

Dynamic Testing helps verify software functionality by executing the program and identifying defects using Black Box and White Box testing techniques.


# Additional Notes – Dynamic Testing

---

# Cyclomatic Complexity

Cyclomatic Complexity measures the logical complexity of a program.

It helps determine:
- Number of independent paths
- Minimum number of test cases needed

---

## Complexity of a Flow Graph `G`

Cyclomatic Complexity `V(G)` can be calculated in three ways:

### Method 1
```text
V(G) = Number of closed regions + 1
```

### Method 2
```text
V(G) = E - N + 2
```

Where:
- E = Number of edges
- N = Number of nodes

### Method 3
```text
V(G) = P + 1
```

Where:
- P = Number of predicate nodes (conditions)

---

# Steps Involved in Basis Path Testing

1. Define basis set of execution paths
2. Determine independent paths
3. Remove infeasible paths
4. Design test cases for basis paths

---

# Basis Path Testing Example – If Else

## Sample Code

```c
main()
{
   int a,b;

   scanf("%d%d",&a,&b);

   if(a>b)
      printf("a is greater");
   else
      printf("b is greater");
}
```

---

## Flow Graph Paths

### Path 1
```text
1 → 2 → 3 → 5
```

Example:
```text
a = 10, b = 5
```

### Path 2
```text
1 → 2 → 4 → 5
```

Example:
```text
a = 2, b = 6
```

---

## McCabe’s Number

### Using Predicate Nodes
```text
P + 1 = 2
```

### Using Formula
```text
E - N + 2 = 5 - 5 + 2 = 2
```

### Using Regions
```text
R + 1 = 2
```

So,

```text
Cyclomatic Complexity = 2
```

---

# Basis Path Testing Example – Loop

## Sample Code

```c
int main()
{
   int n,i;

   scanf("%d",&n);

   for(i=1;i<=n;i++)
   {
      printf("%d",i);
   }
}
```

---

## Independent Paths

### Path 1
```text
1 → 2 → 3 → 4 → 5 → 3 → 4 → 5 → 3 → 6
```

When:
```text
n = 2
```

---

### Path 2
```text
1 → 2 → 3 → 6
```

When:
```text
n = 0
```

---

## McCabe’s Number

### Formula Method
```text
E - N + 2 = 6 - 6 + 2 = 2
```

### Predicate Method
```text
P + 1 = 2
```

### Region Method
```text
R + 1 = 2
```

Therefore,

```text
Cyclomatic Complexity = 2
```

---

# Black Box Testing vs White Box Testing

| Black Box Testing | White Box Testing |
|---|---|
| Focuses on functionality | Focuses on internal logic |
| No knowledge of code needed | Knowledge of code required |
| Finds missing functionality | Finds unreachable code |
| Input/output based | Structure based |
| Performed by testers | Usually performed by developers/testers |

---

## Black Box Techniques
- Equivalence Class Partitioning
- Boundary Value Analysis
- Cause Effect Analysis
- Decision Table Testing
- State Transition Testing

---

## White Box Techniques
- Basis Path Testing
- Statement Coverage
- Branch Coverage
- Loop Coverage

---

# Static Testing vs Dynamic Testing

| Static Testing | Dynamic Testing |
|---|---|
| Code is not executed | Code is executed |
| Finds defects early | Finds runtime defects |
| Manual review process | Actual testing process |
| Less expensive to fix bugs | More expensive than static testing |

---

## Static Testing Techniques
- Review
- Inspection
- Walkthrough

---

## Dynamic Testing Techniques
- Black Box Testing
- White Box Testing

---

# Key Differences

## Static Testing
- Done before execution
- Checks documents and code manually
- Prevents defects early

## Dynamic Testing
- Done after development
- Executes software
- Detects runtime errors

---

# Important Formulas

## Statement Coverage
```text
(Number of executed statements / Total statements) × 100
```

---

## Branch Coverage
```text
(Number of branches covered / Total branches) × 100
```

---

## Cyclomatic Complexity
```text
V(G) = E - N + 2
```

OR

```text
V(G) = P + 1
```

---

# Interview Questions

1. What is Cyclomatic Complexity?
2. Explain McCabe’s Number.
3. Difference between Static and Dynamic Testing?
4. Difference between Black Box and White Box Testing?
5. What is Basis Path Testing?
6. Explain Branch Coverage.
7. What are independent paths?
8. Explain Loop Coverage with example.
9. How is Cyclomatic Complexity calculated?
10. What are predicate nodes?

---

# Conclusion

Dynamic Testing ensures software quality by validating both:
- Functional behavior using Black Box Testing
- Internal code structure using White Box Testing

Basis Path Testing and Cyclomatic Complexity help measure code complexity and design effective test cases.
