# Pseudocode Using Loops - MCQ Questions & Detailed Answers

---

# Question 1
## Match the appropriate opening and closing blocks in looping statements.

| Opening Block | Closing Block |
|---|---|
| WHILE | END WHILE |
| BEGIN | END |
| IF | END IF |
| FOR | END FOR |

## Detailed Explanation
In pseudocode, every control structure must be properly closed.

- `WHILE` loop ends with `END WHILE`
- `FOR` loop ends with `END FOR`
- `IF` condition ends with `END IF`
- Main block begins with `BEGIN` and ends with `END`

These help make the logic readable and organized.

---

# Question 2
## Which looping logic is exit controlled?

### Options
- a. do-while loop
- b. While loop
- c. For loop

## Correct Answer
✅ a. do-while loop

## Detailed Explanation
A do-while loop is called an exit-controlled loop because:

- The statements inside the loop execute first.
- The condition is checked only after execution.

Example:
```text
do
   print "Hello"
while(condition)
```

Even if the condition is false initially, the loop executes once.

---

# Question 3
## Choose the correct statement to complete the pseudocode for factorial calculation.

### Pseudocode
```text
BEGIN
DECLARE variables i, factorial
SET factorial <-- 1

FOR i <-- 1 to 5 do
    ____________
    i <-- i+1
END FOR

PRINT factorial
END
```

### Options
- a. factorial <-- factorial + i
- b. factorial <-- factorial * i
- c. factorial <-- i
- d. factorial <-- factorial - i

## Correct Answer
✅ b. factorial <-- factorial * i

## Detailed Explanation
Factorial means multiplying all numbers from 1 to the given number.

Example:
```text
5! = 1 × 2 × 3 × 4 × 5 = 120
```

The loop multiplies the current factorial value with `i`.

Execution:
```text
1 × 1 = 1
1 × 2 = 2
2 × 3 = 6
6 × 4 = 24
24 × 5 = 120
```

Final Output:
```text
120
```

---

# Question 4
## Consider the output:
```text
0, 2, 4, 6, 8, 10, 12, 16
```

Which pseudocode snippet gives the above output?

### Options

### a.
```text
BEGIN
DECLARE number, count, even
SET count <-- 8, number <-- 0, even <-- 0

WHILE number<count
    PRINT even
    SET even <-- even + 2
    number <-- number + 1
END WHILE

PRINT even
END
```

### b.
```text
BEGIN
DECLARE number, count, even
SET count <-- 16, number <-- 0, even <-- 0

WHILE number<count
    PRINT even
    SET even <-- even + 2
END WHILE
```

### c.
```text
BEGIN
DECLARE number, count, even
SET count <-- 8, number <-- 0, even <-- 0

WHILE number<count
    PRINT even
    SET even <-- even + 1
    number <-- number + 1
END WHILE

PRINT even
END
```

### d.
```text
BEGIN
DECLARE number, count, even
SET count <-- 8, number <-- 0, even <-- 0

WHILE number<count
    PRINT even
    SET even <-- even + 2
    number <-- number + 2
END WHILE
END
```

## Correct Answer
✅ a

## Detailed Explanation
Option (a) correctly:
- Starts from 0
- Adds 2 repeatedly
- Prints even numbers

Execution:
```text
0
2
4
6
8
10
12
14
16
```

---

# Question 5
## Predict the output of the flowchart.

### Flowchart Logic
```text
count = 1
Print count
count = count + 1

If count >= 10
    Stop
Else
    Print count
```

## Options
- a.
```text
2
2
```

- b.
```text
2
1
```

- c.
```text
1
2
```

- d.
```text
1
1
```

## Correct Answer
✅ c. 1 2

## Detailed Explanation
Step-by-step execution:

1. `count = 1`
2. First print → `1`
3. `count = count + 1`
   → count becomes `2`
4. Check:
```text
2 >= 10 → False
```
5. Second print → `2`

Final Output:
```text
1
2
```

---

# Question 6
## Iteration/looping is a repetition of _________

### Options
- a. Block of statements
- b. operation
- c. variables
- d. single statement

## Correct Answers
✅ a. Block of statements  
✅ d. single statement

## Detailed Explanation
Looping means executing instructions repeatedly.

A loop may repeat:
- One statement
- Multiple statements

Example:
```text
PRINT "Hello"
```

or

```text
x = x + 1
PRINT x
```

---

# Question 7
## Do-while looping statement is almost same as ______

### Options
- a. Nested if
- b. if-else
- c. for loop
- d. While loop

## Correct Answer
✅ d. While loop

## Detailed Explanation
Both loops work based on conditions.

Difference:

| While Loop | Do-While Loop |
|---|---|
| Checks condition first | Executes first |
| May execute zero times | Executes at least once |

---

# Question 8
## What is true about FOR LOOP?

### Options
- a. For loop cannot be nested
- b. In for loop, the exact number of iterations is known
- c. For loop executes without checking condition
- d. Executes at least once even if condition is false

## Correct Answer
✅ b. In for loop, the exact number of iterations is known

## Detailed Explanation
For loop is mainly used when:
- Number of repetitions is already known.

Example:
```text
FOR i = 1 to 10
```

This loop runs exactly 10 times.

---

# Question 9
## Flight ticket booking for 5 family members is an example of which loop?

### Options
- a. For loop
- b. Do-while loop
- c. While loop

## Correct Answer
✅ a. For loop

## Detailed Explanation
The process repeats exactly 5 times.

When repetition count is fixed, for loop is best.

---

# Question 10
## What will be the output for WHILE loop?

### Pseudocode
```text
BEGIN
DECLARE number

SET number <-- 30

WHILE number > 0
    number <-- number - 4
END WHILE

PRINT number
END
```

### Options
- a. 0
- b. 2
- c. -2
- d. 4

## Correct Answer
✅ c. -2

## Detailed Explanation
Execution:

```text
30
26
22
18
14
10
6
2
-2
```

When number becomes `-2`,
condition becomes false.

Final Output:
```text
-2
```

---

# Question 11
## What is the output for FOR-loop snippet?

### Code
```text
FOR i <-- 1 to 15
    PRINT i
    i <-- i + 3
END FOR
```

### Options
- a. 4 7 10 13 16
- b. 1 4 7 10 13 15 16
- c. 1 4 7 10 13
- d. 4 7 10 13

## Correct Answer
✅ c. 1 4 7 10 13

## Detailed Explanation
Execution:

```text
i = 1 → print 1
i = i + 3 → 4

i = 4 → print 4
i = 7 → print 7
i = 10 → print 10
i = 13 → print 13
```

Next becomes 16 which is greater than 15.

Loop stops.

---

# Question 12
## Which symbol is inappropriate in sequential flowchart?

### Options
- a. rectangle
- b. oval
- c. parallelogram
- d. diamond

## Correct Answer
✅ d. diamond

## Detailed Explanation
Diamond symbol represents decision making.

Sequential flow does not require conditions.

---

# Question 13
## The statements within the loop must get executed at least once except for do-while statement.

### Options
- True
- False

## Correct Answer
✅ False

## Detailed Explanation
Do-while loop always executes at least once.

Hence the statement is false.

---

# Question 14
## Which statements are true with respect to looping statements?

### Options
- a. initial condition must be applied before execution
- b. loop should run infinite times
- c. termination condition must be given
- d. conditional statements are not allowed

## Correct Answers
✅ a  
✅ c

## Detailed Explanation
Loops need:
- Initialization
- Stopping condition

Infinite loops are usually errors unless intentionally designed.

---

# Question 15
## Which statements are true?

### Options
- a. operand must always be variable
- b. operand must always be constant
- c. operand can be variable or constant
- d. operand is mandatory in an expression

## Correct Answers
✅ c  
✅ d

## Detailed Explanation
Example:
```text
a + 5
```

Operands:
- `a`
- `5`

Operator:
- `+`

---

# Question 16
## Rubik cube solving is an example of which loop?

### Options
- a. Do-while
- b. Nested-if
- c. While
- d. For

## Correct Answer
✅ c. While

## Detailed Explanation
You continue rotating until the cube is solved.

Number of repetitions is unknown.

---

# Question 17
## Crossword Puzzle

### Questions

### Down
1. Step by step list of instructions  
4. When you know exact number of iterations, this loop is used

### Across
2. When process/actions are repeated, these statements are used  
3. Each execution of loop statements is called ______  
5. This loop statement is also called exit-controlled loop

## Answers

| Number | Answer |
|---|---|
| 1 | Algorithm |
| 2 | Looping |
| 3 | Iteration |
| 4 | For |
| 5 | DoWhile |

## Detailed Explanation
- Algorithm → step-by-step procedure
- Looping → repeated execution
- Iteration → one repetition
- For → fixed iteration loop
- DoWhile → exit-controlled loop

---

# Question 18
## Identify the logic which suits the flowchart.

### Options
- a. for loop
- b. nested loop
- c. do-while loop
- d. while loop

## Correct Answer
✅ d. while loop

## Detailed Explanation
Condition is checked before execution.

Hence it is an entry-controlled loop.

---

# Question 19
## Arrange the sequence for Halloween candy collection activity.

### Statements
1. BEGIN  
2. SET candy_count <-- 0  
3. END WHILE  
4. DECLARE candy_count  
5. WHILE candy_count <= 100  
6. candy_count <-- candy_count + 2  
7. END

## Options
- a. 1 2 4 3 6 5 7
- b. 1 4 2 5 6 3 7
- c. 1 4 2 5 6 7 3
- d. 1 4 2 3 6 5 7

## Correct Answer
✅ b. 1 4 2 5 6 3 7

## Detailed Explanation
Steps:
- Start program
- Declare variable
- Initialize variable
- Start loop
- Increment candies
- End loop
- End program

---

# Question 20
## Looping statements are also called ________

### Options
- a. Iteration logic
- b. Sequence logic
- c. Selection logic
- d. Program logic

## Correct Answer
✅ a. Iteration logic

## Detailed Explanation
Looping means repeating instructions repeatedly.

Hence it is also called iteration logic.
