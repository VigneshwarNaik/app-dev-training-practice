# 🔁 Looping Statements 

Looping statements are used to execute a block of code repeatedly until a condition becomes false. They help reduce repeated code and make programs efficient and easy to manage.

---

# 📚 Table of Contents

- Introduction
- Objectives
- Flow of a Program
- What are Looping Statements?
- Types of Looping Statements
- FOR Loop
- WHILE Loop
- DO-WHILE Loop
- Nested Loop
- Difference Between Loops
- Real-Time Uses of Loops
- Conclusion

---

# 📖 Introduction

In programming, sometimes we need to execute the same set of statements multiple times. Writing the same code repeatedly increases complexity and makes programs lengthy.

Looping statements solve this problem by repeating statements automatically based on conditions.

---

# 🎯 Objectives

After completing this module, you will be able to:

- Apply looping statements for simple problems
- Construct looping structures
- Understand different types of loops
- Write algorithms, flowcharts, and pseudocode
- Perform dry run analysis of loops

---

# 🔄 Flow of a Program

The flow of a program is the order in which a computer executes instructions.

Programs are executed in a well-defined manner.

By default, the flow of a program is:

```text
Top to Bottom
```

Program flow can be:

1. Sequential
2. Selective
3. Iterative

---

# 🔁 What are Looping Statements?

Looping statements are used to repeat a block of statements multiple times based on a condition.

They are also called:

```text
Iteration Statements
```

---

# ✅ Advantages of Looping Statements

- Reduces repeated code
- Saves time and memory
- Makes programs smaller
- Improves readability
- Simplifies problem solving

---

# 🧩 Types of Looping Statements

1. FOR Loop
2. WHILE Loop
3. DO-WHILE Loop
4. Nested Loop

---

# 🔹 FOR Loop

## 📖 Definition

FOR loop is used when the number of iterations is already known.

It is an:

```text
Entry-Controlled Loop
```

because the condition is checked before entering the loop body.

---

# ✅ Features of FOR Loop

- Used for fixed number of iterations
- Condition checked before execution
- Executes zero or more times
- Easy to use for counting operations

---

# 🧠 Syntax of FOR Loop

```text
FOR(condition)
DO
    statements
END FOR
```

---

# 📝 Algorithm for FOR Loop

## Problem

Find the sum of marks of 4 subjects.

## Steps

1. Start the process
2. Set i = 0 and sum = 0
3. Check whether i < 4
4. Read number
5. Add number to sum
6. Increment i
7. Print sum
8. Stop the process

---

# 🔄 Flow of FOR Loop

```text
Start
   ↓
Initialize
   ↓
Condition Check
   ↓
Code Block
   ↓
Increment
   ↓
Condition Check Again
```

---

# 💻 Pseudocode for FOR Loop

```text
BEGIN

DECLARE variables i, sum, number

SET i = 0, sum = 0

FOR i = 0 TO 3 DO

    READ number

    sum = sum + number

END FOR

PRINT sum

END
```

---

# 🧪 Dry Run of FOR Loop

## Input

```text
50
80
75
80
```

## Calculation

```text
50 + 80 + 75 + 80 = 285
```

## Output

```text
285
```

---

# 🔹 WHILE Loop

## 📖 Definition

WHILE loop executes statements while the condition remains true.

It is also an:

```text
Entry-Controlled Loop
```

---

# ✅ Features of WHILE Loop

- Condition checked before execution
- Executes zero or more times
- Used when iterations are unknown
- Best for condition-based repetition

---

# 🧠 Syntax of WHILE Loop

```text
WHILE(condition)
DO
    statements
END WHILE
```

---

# 📝 Algorithm for WHILE Loop

## Problem

Print number only if the number is greater than 0.

## Steps

1. Start the process
2. Read number
3. Check whether number > 0
4. Print number
5. Repeat steps
6. Stop process

---

# 🔄 Flow of WHILE Loop

```text
Start
   ↓
Read Number
   ↓
Condition Check
   ↓
Print Number
   ↓
Repeat
```

---

# 💻 Pseudocode for WHILE Loop

```text
BEGIN

DECLARE variable number

READ number

WHILE number > 0

    PRINT number

    READ number

END WHILE

END
```

---

# 🧪 Dry Run of WHILE Loop

## Input

```text
3
-7
```

## Output

```text
3
```

## Explanation

- 3 satisfies condition number > 0
- -7 fails condition
- Loop terminates

---

# 🔹 DO-WHILE Loop

## 📖 Definition

DO-WHILE loop executes the statements first and checks the condition later.

It is called:

```text
Exit-Controlled Loop
```

because the condition is checked after execution.

---

# ✅ Features of DO-WHILE Loop

- Executes at least one time
- Condition checked after execution
- Suitable when code must run once

---

# 🧠 Syntax of DO-WHILE Loop

```text
DO
    statements
WHILE(condition)
```

---

# 📝 Algorithm for DO-WHILE Loop

## Problem

Print number at least once before checking condition.

## Steps

1. Start the process
2. Read number
3. Print number
4. Check whether number < 6
5. Repeat if condition is true
6. Stop process

---

# 🔄 Flow of DO-WHILE Loop

```text
Start
   ↓
Read Number
   ↓
Print Number
   ↓
Condition Check
   ↓
Repeat or Stop
```

---

# 💻 Pseudocode for DO-WHILE Loop

```text
BEGIN

DECLARE variable number

DO

    READ number

    PRINT number

WHILE number < 6

END
```

---

# 🔹 Nested Loop

## 📖 Definition

A loop inside another loop is called a nested loop.

Example:

- FOR loop inside FOR loop
- WHILE loop inside FOR loop
- DO-WHILE inside WHILE loop

---

# ✅ Features of Nested Loop

1. Outer loop executes first
2. Inner loop executes completely
3. Used for pattern problems
4. Useful for matrices and tables

---

# 💻 Pseudocode for Nested FOR Loop

```text
BEGIN

DECLARE variables i, j, size

SET size = 3

FOR i = 0 TO size DO

    FOR j = 0 TO (i + 1) DO

        PRINT "*"

    END FOR

    PRINT newline

END FOR

END
```

---

# 🧪 Output Pattern

```text
*
**
***
****
```

---

# 📊 Difference Between Loop Types

| Loop Type | Condition Check | Executes At Least Once | Best Used When |
|---|---|---|---|
| FOR Loop | Before execution | No | Iterations are known |
| WHILE Loop | Before execution | No | Iterations are unknown |
| DO-WHILE Loop | After execution | Yes | Execution required at least once |

---

# 🌍 Real-Time Uses of Loops

## FOR Loop

- Printing numbers
- Array traversal
- Calculating sums
- Table generation

---

## WHILE Loop

- Password validation
- Menu-driven programs
- Reading inputs continuously

---

## DO-WHILE Loop

- ATM machine operations
- Game menus
- User choice repetition

---

## Nested Loops

- Pattern printing
- Matrix operations
- Chess board generation

---

# 📌 Important Points

- FOR loop is best for fixed repetitions
- WHILE loop is best for unknown repetitions
- DO-WHILE loop executes at least once
- Nested loops are used for complex repetition problems

---

# 🏁 Conclusion

Looping statements are an important part of programming. They help automate repetitive tasks and reduce code duplication.

Understanding:

- FOR Loop
- WHILE Loop
- DO-WHILE Loop
- Nested Loop

is essential for building strong programming logic and solving real-world problems efficiently.

---

# 
