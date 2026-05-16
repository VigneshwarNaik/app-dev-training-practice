# Selection Statements

## Introduction

Selection statements are used in programming to make decisions based on conditions.

They help control the flow of execution of a program.

Selection statements are also called:

- Conditional Statements
- Decision-Making Statements

---

# Table of Contents

- Introduction
- Objectives
- Flow of Program
- Types of Selection Statements
- Difference Between Selection Statements
- Simple If
- If-Else
- Else-If Ladder
- Nested If
- Real-Time Examples
- Advantages
- Conclusion

---

# Objectives

After completing this module, you will be able to:

- Apply selection statements for simple problems
- Construct decision-making statements
- Understand program flow

---

# Flow of a Program

A program executes statements in a specific order.

## Important Points

1. Programs are executed in a well-defined manner.
2. By default, execution happens from top to bottom.
3. Program flow can be:
   - Sequential
   - Selective
   - Iterative

---

# Types of Selection Statements

1. Simple If
2. If-Else
3. Else-If Ladder
4. Nested If

---

# Difference Between Selection Statements

| Statement | Purpose |
|---|---|
| Simple If | Executes only if condition is true |
| If-Else | Chooses between two blocks |
| Else-If Ladder | Checks multiple conditions |
| Nested If | Checks condition inside another condition |

---

# 1. Simple If Statement

## Definition

Simple if statement executes statements only when the condition is TRUE.

---

## Syntax

```text
IF(condition)
   statement
ENDIF
```

---

## Working

- If condition is TRUE:
  - Statements inside if block execute
- If condition is FALSE:
  - Statements are skipped

---

## Example

```text
IF(number < 6)
   PRINT square
ENDIF
```

---

## Algorithm

```text
STEP 1: Start
STEP 2: Read number
STEP 3: Check number < 6
STEP 4: Square the number
STEP 5: Print result
STEP 6: Stop
```

---

## Flowchart

```text
Start
  ↓
Read Number
  ↓
number < 6 ?
  ↓ YES
Square Number
  ↓
Print Result
  ↓
Stop
```

---

## Dry Run

### Input = 5

| Step | Number | Condition | Output |
|------|---------|------------|---------|
| 1 | 5 | TRUE | 25 |

### Input = 15

| Step | Number | Condition | Output |
|------|---------|------------|---------|
| 1 | 15 | FALSE | No Output |

---

# 2. If-Else Statement

## Definition

If-Else statement executes one among two blocks depending on the condition.

---

## Syntax

```text
IF(condition)
   statement
ELSE
   statement
ENDIF
```

---

## Working

- If condition is TRUE:
  - if block executes
- If condition is FALSE:
  - else block executes

---

## Example

Check whether a number is EVEN or ODD.

---

## Algorithm

```text
STEP 1: Start
STEP 2: Read number
STEP 3: Check number % 2 == 0
STEP 4: Print EVEN
STEP 5: Print ODD
STEP 6: Stop
```

---

## Flowchart

```text
Start
  ↓
Read Number
  ↓
number % 2 == 0 ?
  ↓ YES          ↓ NO
Print EVEN     Print ODD
       ↓
      Stop
```

---

## Pseudocode

```text
BEGIN

READ number

IF(number % 2 == 0)
   PRINT "EVEN"
ELSE
   PRINT "ODD"
ENDIF

END
```

---

## Dry Run

### Input = 5

| Number | Condition | Output |
|---------|------------|---------|
| 5 | FALSE | ODD |

### Input = 8

| Number | Condition | Output |
|---------|------------|---------|
| 8 | TRUE | EVEN |

---

# 3. Else-If Ladder

## Definition

Else-if ladder is used when multiple conditions are checked one after another.

---

## Working

- Conditions are checked sequentially
- First TRUE condition executes
- Remaining conditions are skipped
- If all conditions are FALSE:
  - else block executes

---

## Syntax

```text
IF(condition1)
   statement

ELSE IF(condition2)
   statement

ELSE IF(condition3)
   statement

ELSE
   statement

ENDIF
```

---

## Example

Find grade based on average marks.

---

## Algorithm

```text
STEP 1: Start
STEP 2: Read average

STEP 3:
If average >= 90
Grade = A

STEP 4:
Else if average >= 70
Grade = B

STEP 5:
Else if average >= 50
Grade = C

STEP 6:
Else
Grade = D

STEP 7:
Print Grade

STEP 8:
Stop
```

---

## Flowchart

```text
Start
  ↓
Read Average
  ↓
average >= 90 ?
  ↓YES
Print A

NO ↓
average >= 70 ?
  ↓YES
Print B

NO ↓
average >= 50 ?
  ↓YES
Print C

NO ↓
Print D
  ↓
Stop
```

---

## Pseudocode

```text
BEGIN

READ average

IF average >= 90
   PRINT "A"

ELSE IF average >= 70
   PRINT "B"

ELSE IF average >= 50
   PRINT "C"

ELSE
   PRINT "D"

ENDIF

END
```

---

## Dry Run

### Input = 85

| Average | Condition Matched | Output |
|----------|------------------|---------|
| 85 | average >= 70 | B |

---

# 4. Nested If Statement

## Definition

Nested if means an if statement inside another if statement.

Used when one condition depends on another condition.

---

## Syntax

```text
IF(condition1)

   IF(condition2)
      statement
   ELSE
      statement
   ENDIF

ELSE
   statement

ENDIF
```

---

## Example

Check eligibility for driving license.

Conditions:
- Age must be above 18
- Person must pass driving test

---

## Algorithm

```text
STEP 1: Start
STEP 2: Read age
STEP 3: Check age >= 18

STEP 4:
If TRUE
   Check driving test result

STEP 5:
If pass
   Print Eligible

STEP 6:
Else
   Print Not Eligible

STEP 7:
Else
   Print Under Age

STEP 8:
Stop
```

---

## Flowchart

```text
Start
  ↓
Read Age
  ↓
Age >= 18 ?
  ↓YES                ↓NO
Driving Test?       Under Age
  ↓YES    ↓NO
Eligible  Not Eligible
      ↓
     Stop
```

---

## Pseudocode

```text
BEGIN

READ age

IF age >= 18

   READ testResult

   IF testResult == "PASS"
      PRINT "Eligible"

   ELSE
      PRINT "Not Eligible"

   ENDIF

ELSE
   PRINT "Under Age"

ENDIF

END
```

---

## Dry Run

### Input

```text
Age = 20
TestResult = PASS
```

### Output

```text
Eligible
```

---

# Real-Time Examples of Selection Statements

| Application | Use |
|---|---|
| ATM Machine | Balance checking |
| Login System | Username/password validation |
| Student Result | Grade calculation |
| Traffic Signal | Signal checking |
| Online Shopping | Payment verification |

---

# Advantages of Selection Statements

- Helps in decision making
- Controls program flow
- Reduces unnecessary execution
- Makes programs smarter
- Improves logical thinking

---

# Conclusion

Selection statements are important programming concepts used for decision making.

Main types:

1. Simple If
2. If-Else
3. Else-If Ladder
4. Nested If

They help programs execute different actions based on conditions and improve logical problem solving.

---
