# Arrays


---

# 📚 Table of Contents

1. Introduction
2. What is an Array?
3. Features of Arrays
4. One-Dimensional Array
5. Algorithm for 1D Array
6. Pseudocode for 1D Array
7. Finding Maximum Element
8. Compatible Arrays
9. Two-Dimensional Arrays
10. Algorithm for 2D Array
11. Pseudocode for 2D Array
12. Searching in Arrays
13. Linear Search
14. Sorting
15. Bubble Sort
16. Time Complexity
17. Advantages and Disadvantages
18. Conclusion

---

# 📘 Introduction

Arrays are one of the most important data structures in programming.

An array is used to store multiple values of the same datatype in contiguous memory locations.

Arrays make storing, accessing, searching, and sorting data easier and faster.

---

# ❓ What is an Array?

An array is a collection of homogeneous data stored sequentially.

## Definition

```text
An array is a variable used to store multiple values of the same datatype continuously.
```

---

# ✨ Features of Arrays

- Stores elements of the same datatype
- Elements are stored sequentially
- Arrays have fixed size
- Fast access using index
- Easy to traverse
- Supports searching and sorting

---

# 🌍 Real-Life Examples of Arrays

| Example | Description |
|---|---|
| Student Marks | Store marks of students |
| Employee IDs | Store employee numbers |
| Product Prices | Store product costs |
| Temperatures | Store daily temperatures |

---

# 📦 One-Dimensional Array (1D Array)

A one-dimensional array stores elements in a single row.

## Example

```text
marks[5]
```

---

## 📊 Representation

| Index | 0 | 1 | 2 | 3 | 4 |
|---|---|---|---|---|---|
| Value | 90 | 85 | 76 | 95 | 88 |

---

## Important Points

- Index starts from `0`
- Last index is `n - 1`
- Access elements using:

```text
array_name[index]
```

### Example

```text
marks[0] = 90
```

---

# 🧠 Algorithm for 1D Array

## Problem Statement

Read marks of 5 students and print average marks.

---

## Algorithm Steps

### Step 1
Start the process

### Step 2
Create array:

```text
marks[5]
```

### Step 3
Initialize:

```text
sum = 0
index = 0
```

### Step 4
Check:

```text
index < 5
```

If YES → Step 5  
If NO → Step 7

### Step 5
Read:

```text
marks[index]
```

### Step 6
Add:

```text
sum = sum + marks[index]
```

Increment:

```text
index = index + 1
```

Go to Step 4

### Step 7
Calculate average:

```text
average = sum / 5
```

### Step 8
Display average

### Step 9
Stop the process

---

# 💻 Pseudocode for 1D Array

```text
BEGIN

DECLARE index, sum, average, marks[5]

SET index = 0
SET sum = 0

FOR index ← 0 to 4 DO

    READ marks[index]

    sum ← sum + marks[index]

END FOR

average ← sum / 5

PRINT average

END
```

---

# 🔍 Finding Maximum Element in Array

## Problem Statement

Find the maximum element in an array.

---

## Pseudocode

```text
BEGIN

DECLARE index, maximum, array[10]

FOR index ← 0 to 9 DO

    READ array[index]

END FOR

SET maximum ← array[0]

FOR index ← 0 to 9 DO

    IF maximum < array[index]

        maximum ← array[index]

    END IF

END FOR

PRINT maximum

END
```

---

# 🤝 Compatible Arrays

Two arrays are compatible if:

- Both arrays have equal size
- Every element in first array is greater than or equal to second array

---

## Example

### Array 1

```text
[2, 3, 8, 6, 1]
```

### Array 2

```text
[1, 1, 1, 1, 1]
```

Compatible ✅

---

# 💻 Pseudocode for Compatible Arrays

```text
BEGIN

DECLARE i, number, a[15], b[15], flag

GET number

SET flag = 0

FOR i ← 0 to number-1 DO

    READ a[i]

END FOR

FOR i ← 0 to number-1 DO

    READ b[i]

END FOR

FOR i ← 0 to number-1 DO

    IF a[i] < b[i]

        SET flag = 1

        BREAK

    END IF

END FOR

IF flag == 0

    PRINT "Compatible"

ELSE

    PRINT "Incompatible"

END

```

---

# 🧩 Two-Dimensional Arrays (2D Arrays)

A two-dimensional array stores elements in rows and columns.

2D arrays are also called arrays of arrays.

---

## Example

```text
marks[3][3]
```

---

# 📊 Representation of 2D Array

| Rows/Columns | Col0 | Col1 | Col2 |
|---|---|---|---|
| Row0 | marks[0][0] | marks[0][1] | marks[0][2] |
| Row1 | marks[1][0] | marks[1][1] | marks[1][2] |
| Row2 | marks[2][0] | marks[2][1] | marks[2][2] |

---

# Accessing Elements in 2D Array

```text
array_name[row][column]
```

### Example

```text
marks[0][0] = 93
```

---

# 🧠 Algorithm for 2D Array

## Problem Statement

Read and display scores of 3 students in 3 subjects.

---

## Algorithm Steps

### Step 1
Create:

```text
marks[3][3]
```

### Step 2
Initialize:

```text
i = 0
j = 0
```

### Step 3
Check:

```text
i < 3
```

### Step 4
Check:

```text
j < 3
```

### Step 5
Read:

```text
marks[i][j]
```

### Step 6
Increment:

```text
j = j + 1
```

### Step 7
Increment:

```text
i = i + 1
```

### Step 8
Display marks

### Step 9
Stop process

---

# 💻 Pseudocode for 2D Array

```text
BEGIN

DECLARE i, j, marks[3][3]

SET i = 0
SET j = 0

FOR i ← 0 to 2 DO

    FOR j ← 0 to 2 DO

        READ marks[i][j]

    END FOR

END FOR

PRINT "STUDENTS SCORES ARE"

FOR i ← 0 to 2 DO

    FOR j ← 0 to 2 DO

        PRINT marks[i][j]

    END FOR

END FOR

END
```

---

# 🖥️ Sample Output for 2D Array

```text
STUDENTS SCORES ARE

Student 1
96
98
95

Student 2
89
97
97

Student 3
99
85
83
```

---

# 🔎 Searching in Arrays

Searching means finding a particular element in a collection.

---

# Linear Search

Linear search checks elements one by one.

---

## Steps in Linear Search

1. Start from first element
2. Compare each element with target
3. If found → return index
4. Else continue searching
5. If not found → display message

---

# 🧠 Algorithm for Searching

### Step 1
Start process

### Step 2
Create array:

```text
employee_id[8]
```

### Step 3
Initialize:

```text
flag = 0
i = 0
```

### Step 4
Read array elements

### Step 5
Read search number

### Step 6
Compare each element

### Step 7
If found:

```text
PRINT "Number Found"
```

### Step 8
Else:

```text
PRINT "Number Not Found"
```

---

# 💻 Linear Search Pseudocode

```text
BEGIN

DECLARE i, n, arr[8], flag

SET flag = 0

FOR i ← 0 to 7 DO

    READ arr[i]

END FOR

READ n

FOR i ← 0 to 7 DO

    IF arr[i] == n THEN

        flag ← 1

        BREAK

    END IF

END FOR

IF flag == 1

    PRINT "Number Found"

ELSE

    PRINT "Number Not Found"

END IF

END
```

---

# 🔃 Sorting

Sorting means arranging elements in a particular order.

---

## Types of Sorting

- Bubble Sort
- Selection Sort
- Insertion Sort
- Exchange Sort

---

# 🫧 Bubble Sort

Bubble sort repeatedly compares adjacent elements and swaps them if they are in wrong order.

---

# 🧠 Bubble Sort Algorithm

### Step 1
Input array elements

### Step 2
Repeat passes through array

### Step 3
Compare adjacent elements

### Step 4
If:

```text
A[j] > A[j+1]
```

swap them

### Step 5
Repeat until sorted

---

# 💻 Bubble Sort Pseudocode

```text
BEGIN

DECLARE i, j, swap, A[n]

FOR i ← 0 to n-1 DO

    FOR j ← 0 to n-i-1 DO

        IF A[j] > A[j+1]

            swap ← A[j]

            A[j] ← A[j+1]

            A[j+1] ← swap

        END IF

    END FOR

END FOR

PRINT sorted array

END
```

---

# ⏱️ Time Complexity

| Operation | Time Complexity |
|---|---|
| Access | O(1) |
| Traversal | O(n) |
| Linear Search | O(n) |
| Bubble Sort | O(n²) |
| Insertion | O(n) |
| Deletion | O(n) |

---

# ✅ Advantages of Arrays

- Fast access using index
- Easy traversal
- Simple implementation
- Useful for storing large data

---

# ❌ Disadvantages of Arrays

- Fixed size
- Wastage of memory possible
- Insertion and deletion difficult
- Cannot store different datatypes together

---

# 🎯 Conclusion

Arrays are one of the most important and basic data structures in programming.

They help in:
- Storing data efficiently
- Searching data
- Sorting data
- Processing large collections of elements

Arrays are widely used in:
- Data Structures
- Algorithms
- Databases
- Applications
- Competitive Programming

---

# 📌 Topics Covered

✅ Arrays  
✅ 1D Arrays  
✅ 2D Arrays  
✅ Algorithms  
✅ Pseudocode  
✅ Linear Search  
✅ Sorting  
✅ Bubble Sort  
✅ Compatible Arrays  
✅ Time Complexity  
✅ Advantages & Disadvantages  

---

