# Dynamic Testing – Post Quiz Questions and Answers

## Question 1

### Question
Determine the cyclomatic complexity for the following code:

```text
Accept year

if(year mod 4=0 and year mod 100!=0) or(year mod 400 =0)

print year is leap

else

print year is not leap

end if
```

### Options
- a. 6
- b. 4
- c. 3
- d. 5

### Correct Answer
✅ **b. 4**

### Explanation
Cyclomatic Complexity is calculated using:

```text
V(G) = P + 1
```

Where:
- P = Number of predicate conditions

Conditions present:
1. year mod 4 = 0
2. year mod 100 != 0
3. year mod 400 = 0

So,

```text
V(G) = 3 + 1 = 4
```

---

# Question 2

### Question
Walk through is performed by the trained moderator, whereas the Inspection is usually conducted by the author itself to record defects and deviations.

### Options
- True
- False

### Correct Answer
✅ **False**

### Explanation
The statement is incorrect because:

- **Walkthrough** → Usually conducted by the author.
- **Inspection** → Conducted by trained moderators or review teams.

---

# Question 3

### Question
The testing technique that deals with the internal logic and structure of the code is called ________.

### Options
- a. Pure Box Testing
- b. Logical Testing
- c. WhiteBox Testing

### Correct Answer
✅ **c. WhiteBox Testing**

### Explanation
White Box Testing focuses on:
- Internal code structure
- Logic of the program
- Statement coverage
- Branch coverage
- Loop coverage

---

# Question 4

### Question
Tester is trying to test whether the values in the drop down are listed properly.

What type of testing the tester performs in this scenario?

### Options
- a. White box Testing
- b. Acceptance Testing
- c. Regression Testing
- d. Black box testing

### Correct Answer
✅ **d. Black box testing**

### Explanation
The tester is validating the functionality visible to the user without checking internal code.

Therefore, it is:
```text
Black Box Testing
```

---

# Question 5

### Question
After implementation of Library management system, the tester identified that certain logic are redundantly rewritten by the developers, and the coding standards are violated in few modules.

What type of testing is carried out to identify these errors?

### Options
- a. error guessing
- b. debugging
- c. dynamic testing
- d. Static Testing

### Correct Answer
✅ **d. Static Testing**

### Explanation
Static Testing is used to:
- Review source code
- Check coding standards
- Identify redundant logic
- Detect issues without executing the program

Examples:
- Review
- Inspection
- Walkthrough

---

# Question 6

### Question
Boundary value analysis can only be used during white-box testing.

State whether True or False.

### Options
- a. FALSE
- b. TRUE

### Correct Answer
✅ **a. FALSE**

### Explanation
Boundary Value Analysis (BVA) is a:
```text
Black Box Testing Technique
```

It tests values at:
- Minimum boundary
- Maximum boundary
- Just below minimum
- Just above maximum

---

# Question 7

### Question
In the online shopping portal, for customer registration the password field can accept only characters in the range of 5 to 25.

Derive test cases using Boundary Value Analysis.

### Options
- a. 5,25,4,26
- b. 5,25,26,3
- c. 6,24,10,25
- d. 5,25,6,24

### Correct Answer
✅ **a. 5,25,4,26**

### Explanation
Boundary Value Analysis checks:
- Minimum value
- Maximum value
- Just below minimum
- Just above maximum

Given range:
```text
5 to 25
```

Test cases:
- 5 → Minimum valid
- 25 → Maximum valid
- 4 → Just below minimum
- 26 → Just above maximum

---

# Summary Table

| Question | Correct Answer |
|---|---|
| Q1 | b. 4 |
| Q2 | False |
| Q3 | c. WhiteBox Testing |
| Q4 | d. Black box testing |
| Q5 | d. Static Testing |
| Q6 | a. FALSE |
| Q7 | a. 5,25,4,26 |

---

# Topics Covered

- Cyclomatic Complexity
- Static Testing
- Dynamic Testing
- White Box Testing
- Black Box Testing
- Boundary Value Analysis
- Code Review Techniques
- Test Case Design

---

# Conclusion

This quiz covers important concepts of:
- Dynamic Testing
- Static Testing
- Black Box Testing
- White Box Testing
- Cyclomatic Complexity
- Boundary Value Analysis

These concepts are widely used in:
- Software Testing Interviews
- QA Testing
- Automation Testing
- Manual Testing
- Software Engineering Exams

```
