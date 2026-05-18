# Check Your Understanding – Detailed Questions and Answers


# Question 1

## Question
Identify this technique of dynamic testing where, for a range of input, three values are chosen:
- One value above the range
- One value below the range
- One value within the range

### Options
- a. Boundary Value Analysis
- b. Cause Effect Graphing
- c. Cause Effect Analysis
- d. Equivalence partitioning
- e. Error Guessing

---

## Correct Answer
✅ **d. Equivalence partitioning**

---

## Explanation
Equivalence Partitioning is a Black Box Testing technique.

It divides the input data into different groups called equivalence classes.

For testing:
- One value below the range
- One value within the range
- One value above the range

are selected.

### Example
If valid marks are between 1 and 100:

| Type | Example |
|---|---|
| Below Range | 0 |
| Within Range | 50 |
| Above Range | 101 |

---

# Question 2

## Question
What is the difference between the actual output of a software and the correct output?

### Options
- a. Defect
- b. Error
- c. Fault
- d. Bug

---

## Correct Answer
✅ **b. Error**

---

## Explanation
An Error is the difference between:
- Actual output
- Expected/Correct output

### Example
Expected Output:
```text
10
```

Actual Output:
```text
8
```

Difference = Error

---

# Question 3

## Question
Match the objectives of the phases of Software Testing Life Cycle.

---

## Correct Answers

| Phase | Objective |
|---|---|
| Test Design | Test scenarios, test cases, test data, and test scripts are prepared |
| Test Execution | Executing test scripts and Finding bugs |
| Test Plan | Resource allocation, creation of test environment, test schedule and test functionality |

---

## Explanation

### Test Plan
Defines:
- Resources
- Schedule
- Environment
- Testing activities

### Test Design
Creates:
- Test cases
- Test data
- Test scripts

### Test Execution
Executes:
- Test cases
- Detects bugs and defects

---

# Question 4

## Question
Match the roles involved in Static Testing.

---

## Correct Answers

| Role | Responsibility |
|---|---|
| Author | Writer of the ‘document under review’ |
| Reader | Presents the document |
| Inspector | Inspecting the document |
| Scribe | Records each defect found |
| Moderator | Leads the review process |

---

## Explanation

### Author
Creates the document or code.

### Reader
Explains and presents the document during review.

### Inspector
Finds defects and mistakes.

### Scribe
Records all identified defects.

### Moderator
Controls and manages the review meeting.

---

# Question 5

## Question
What is the type of testing in which the tester knows only the input and expected output details based on the specification document and has no knowledge about implementation?

### Options
- a. Regression Testing
- b. Integration Testing
- c. White Box Testing
- d. Usability Testing
- e. Black Box Testing

---

## Correct Answer
✅ **e. Black Box Testing**

---

## Explanation
Black Box Testing checks software functionality without seeing internal code.

Tester knows:
- Inputs
- Expected outputs

Tester does not know:
- Internal logic
- Source code

### Example
Login page testing:
- Enter username/password
- Verify successful login

No need to know backend code.

---

# Question 6

## Question
Identify the correct phases of Software Testing Life Cycle.

### Options
- a. Requirements Analysis, Test Preparation, Test Case development, Test Environment Set up, Test Cycle closure, Test Execution
- b. Requirements Analysis, Test Preparation, Test Case development, Test Execution, Test Environment Set up, Test Cycle closure
- c. Requirements Analysis, Test Case development, Test Preparation, Test Environment Set up, Test Execution, Test Cycle closure
- d. Requirements Analysis, Test Preparation, Test Case development, Test Environment Set up, Test Execution, Test Cycle closure

---

## Correct Answer
✅ **d. Requirements Analysis, Test Preparation, Test Case development, Test Environment Set up, Test Execution, Test Cycle closure**

---

## Explanation of STLC Phases

1. Requirements Analysis
2. Test Preparation
3. Test Case Development
4. Test Environment Setup
5. Test Execution
6. Test Cycle Closure

---

# Question 7

## Question
Match the objectives against the techniques of generating test cases in Black Box Testing.

---

## Correct Answers

| Technique | Objective |
|---|---|
| Cause Effect Graphing | The causes and effects represent the nodes |
| State Transition Diagram | Involves actions as one of its components |
| Cause Effect Analysis | It is suitable for applications in which combinations of input conditions are few |

---

## Explanation

### Cause Effect Graphing
Represents:
- Causes = Inputs
- Effects = Outputs

using graph nodes.

### State Transition Diagram
Represents:
- States
- Transitions
- Actions

### Cause Effect Analysis
Useful when:
- Input combinations are limited
- Logical relationships are important

---

# Question 8

## Question
Which all of the following options would Basis Path Testing perform?

### Options
- a. Test Case Coverage
- b. Statement Coverage
- c. Loop Coverage
- d. Condition or Branch Coverage

---

## Correct Answers
✅ b. Statement Coverage  
✅ c. Loop Coverage  
✅ d. Condition or Branch Coverage  

❌ a. Test Case Coverage

---

## Explanation

Basis Path Testing is a White Box Testing technique.

It focuses on:

### Statement Coverage
Executes every statement at least once.

### Loop Coverage
Tests:
- 0 iterations
- 1 iteration
- Multiple iterations

### Condition/Branch Coverage
Checks all conditions as:
- TRUE
- FALSE

### Example
```c
if(a>b)
```

Test Cases:
- a=10, b=5 → TRUE
- a=2, b=8 → FALSE

---
