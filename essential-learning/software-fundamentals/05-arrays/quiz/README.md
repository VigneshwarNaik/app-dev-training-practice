# Pseudocode Using Arrays - Detailed Quiz Questions and Answers

---

# Question 1

## Problem Statement: Dinner Plan

Five friends plan to go out for dinner.  
They decide to order an equal number of dishes.  
Each row in the matrix represents the cost of dishes ordered by one person.

Write the correct pseudocode snippet to calculate the total amount each person needs to pay.

---

# Matrix Values

```text
12 23 18
45 32 60
42 39 23
54 42 60
25 84 30
```

---

# Expected Output

```text
Amount to be paid by person 1 is 53
Amount to be paid by person 2 is 137
Amount to be paid by person 3 is 104
Amount to be paid by person 4 is 156
Amount to be paid by person 5 is 139
```

---

# Explanation

The output is obtained by calculating the sum of each row.

Example:

```text
Person 1:
12 + 23 + 18 = 53

Person 2:
45 + 32 + 60 = 137
```

Each row corresponds to one person.

---

# Incomplete Pseudocode

```text
BEGIN

DECLARE variable arr[5][20], n, sum=0

___________________

   FOR j IN 0 to n-1 DO

       READ arr[i][j]

   END FOR

END FOR

FOR i IN 0 TO 4 DO

    SET sum = 0

    FOR j IN 0 TO n-1 DO

        sum = sum + arr[i][j]

    END FOR

    PRINT "Amount to be paid by person "+(i+1)+" is "+sum

END FOR

END
```

---

# Options

## a.
```text
FOR i IN 0 to n DO
```

## b.
```text
FOR i IN 0 to 4 DO
```

## c.
```text
FOR i IN 0 to 3 DO
```

## d.
```text
FOR i IN 0 to 5 DO
```

---

# Correct Answer

✅ **b. FOR i IN 0 to 4 DO**

---

# Detailed Explanation

There are 5 friends.

The array is:

```text
arr[5][20]
```

This means:
- 5 rows
- Each row represents one person

Indexes in arrays start from `0`.

So valid indexes are:

| Person | Index |
|---|---|
| Person 1 | 0 |
| Person 2 | 1 |
| Person 3 | 2 |
| Person 4 | 3 |
| Person 5 | 4 |

Therefore, the loop should run from:

```text
0 to 4
```

to process all 5 persons.

---

# Why Other Options Are Wrong

## Option a
```text
FOR i IN 0 to n DO
```

❌ Incorrect because:
- `n` represents number of dishes (columns)
- Not number of persons (rows)

---

## Option c
```text
FOR i IN 0 to 3 DO
```

❌ Processes only 4 persons.

---

## Option d
```text
FOR i IN 0 to 5 DO
```

❌ Accesses invalid index.

Maximum valid index is `4`.

This may cause out-of-bound error.

---

# Final Answer

✅ **b. FOR i IN 0 to 4 DO**

---

---

# Question 2

## Problem Statement: Find Maximum Value

Choose the correct pseudocode to find the maximum value in each row of a matrix.

Assume the matrix is `3 × 3`.

---

# Matrix Representation

```text
(0,0) (0,1) (0,2)
(1,0) (1,1) (1,2)
(2,0) (2,1) (2,2)
```

---

# Matrix Values

```text
12 23 18
45 32 60
42 39 23
```

---

# Expected Output

```text
Max value in row 1 is 23
Max value in row 2 is 60
Max value in row 3 is 42
```

---

# Explanation

For each row:
- Compare all elements
- Find the largest element
- Print the maximum value

Example:

### Row 1
```text
12 23 18
```

Maximum = `23`

### Row 2
```text
45 32 60
```

Maximum = `60`

### Row 3
```text
42 39 23
```

Maximum = `42`

---

# Options

## Option a

```text
BEGIN

DECLARE variable arr[3][3]

FOR i IN 0 to 2 DO

   FOR j IN 0 to 2 DO

       READ arr[i][j]

   END FOR

END FOR

FOR i IN 0 TO 2 DO

SET max = arr[i][0]

FOR j IN 0 TO 2 DO

IF arr[i][j]>max THEN

max = arr[i][j]

END IF

END FOR

END FOR

PRINT "Max value in row "+(i+1)+" is "+max

END
```

---

## Option b

```text
BEGIN

DECLARE variable arr[3][3]

FOR i IN 0 to 2 DO

   FOR j IN 0 to 2 DO

       READ arr[i][j]

   END FOR

END FOR

SET max = arr[i][0]

FOR i IN 0 TO 2 DO

FOR j IN 0 TO 2 DO

IF arr[i][j]>max THEN

max = arr[i][j]

END IF

END FOR

PRINT "Max value in row "+(i+1)+" is "+max

END FOR

END
```

---

## Option c

```text
BEGIN

DECLARE variable arr[3][3]

FOR i IN 0 to 2 DO

   FOR j IN 0 to 2 DO

END FOR

END FOR

FOR i IN 0 TO 2 DO

READ arr[i][j]

SET max = arr[i][0]

FOR j IN 0 TO 2 DO

IF arr[i][j]>max THEN

max = arr[i][j]

END IF

END FOR

PRINT "Max value in row "+(i+1)+" is "+max

END FOR

END
```

---

## Option d

```text
BEGIN

DECLARE variable arr[3][3]

FOR i IN 0 to 2 DO

   FOR j IN 0 to 2 DO

       READ arr[i][j]

   END FOR

END FOR

FOR i IN 0 TO 2 DO

SET max = arr[i][0]

FOR j IN 0 TO 2 DO

IF arr[i][j]>max THEN

max = arr[i][j]

END IF

END FOR

PRINT "Max value in row "+(i+1)+" is "+max

END FOR

END
```

---

# Correct Answer

✅ **d.**

---

# Detailed Explanation

The pseudocode should:

1. Read all matrix values
2. Traverse each row
3. Assume first element is maximum
4. Compare remaining elements
5. Update maximum when larger element found
6. Print row-wise maximum

---

# Important Logic

## Step 1
Initialize maximum:

```text
SET max = arr[i][0]
```

This assumes first element of row is maximum.

---

## Step 2
Compare all elements:

```text
IF arr[i][j] > max
```

If condition is true:
- Update maximum

---

## Step 3
Print maximum after inner loop ends.

---

# Why Option d is Correct

✔ Reads matrix correctly  
✔ Finds maximum for each row separately  
✔ Resets maximum for every row  
✔ Prints output row-wise

---

# Why Other Options Are Wrong

## Option a

❌ `PRINT` statement is outside outer loop.

Only last row maximum gets printed.

---

## Option b

❌ `SET max = arr[i][0]` is outside loop.

This causes incorrect logic.

It finds overall maximum instead of row-wise maximum.

---

## Option c

❌ Matrix values are not read properly.

`READ arr[i][j]` is outside nested loop.

---

# Final Answers

| Question | Correct Answer |
|---|---|
| Question 1 | ✅ b |
| Question 2 | ✅ d |
