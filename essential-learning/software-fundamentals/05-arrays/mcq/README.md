# Arrays – Check Your Understanding MCQ

## Question 1
### Copying one array into another array

#### Question
A mathematical quiz contest happened in a school and the scores are stored in an array named `quizmark`. The coordinating person wants to copy the quiz score into another array named `copyquizmark`. Which option will do that?

### Options

```text
a. copyquizmark <- quizmark
```

```text
b. We cannot copy the values from one array to another
```

```text
c.
FOR index <- 0 to n
    copyquizmark[index] <- quizmark[index]
END FOR
```

```text
d. copyquizmark[n] <- quizmark[n]
```

## Correct Answer
✅ Option c

## Explanation

```text
FOR index <- 0 to n
    copyquizmark[index] <- quizmark[index]
END FOR
```

This loop copies each element one by one from `quizmark` into `copyquizmark`.

- `quizmark[index]` accesses original values.
- `copyquizmark[index]` stores copied values.

### Why other options are wrong?
- a ❌ Copies reference only
- b ❌ Arrays can be copied
- d ❌ Copies only one element

---

# Question 2
## Array Size

### Question

```text
number[100] <- 99
```

How many elements can be stored inside array `number`?

### Options
- a. 99
- b. 100
- c. Infinite number of elements
- d. No clue

## Correct Answer
✅ b. 100

## Explanation

The array size is 100.

Indices are usually:

```text
0 to 99
```

Total elements = 100.

---

# Question 3
## Array Types

| Scenario | Array Type |
|---|---|
| Matrix multiplication | Two-dimensional array |
| Prime number list | One-dimensional array |

## Explanation

### Matrix multiplication

```text
matrix[3][3]
```

Rows and columns require a 2D array.

### Prime numbers list

```text
prime[25]
```

Simple list uses 1D array.

---

# Question 4
## False Statements about Arrays

### Options
- a. It is possible to increase array size
- b. Array can store heterogeneous data
- c. Elements stored contiguously
- d. Arrays store homogeneous data

## Correct Answers
✅ a and b

## Explanation

### a ❌
Arrays have fixed size.

### b ❌
Arrays store same datatype only.

### c ✅
Stored continuously in memory.

### d ✅
Arrays store homogeneous data.

---

# Question 5
## Negative Numbers in Arrays

### Question
Negative elements can be placed inside arrays.

## Correct Answer
✅ True

## Explanation

```text
arr = [-5, -2, 7]
```

Negative values can be stored.

---

# Question 6
## Accessing Array Elements

### Question
5th associate name in:

```text
associate_name[50]
```

### Options
- a. associate_name[6]
- b. associate_name[5]
- c. associate_name[4]
- d. associate_name[3+1]

## Correct Answers
✅ c and d

## Explanation

Arrays start from index 0.

```text
1st element -> index 0
5th element -> index 4
```

---

# Question 7
## Array Declaration

### Question
Information about ______ need not be specified during array declaration.

## Correct Answer
✅ elements to be stored

## Explanation

Example:

```text
int marks[5]
```

Datatype, name, and size are required.
Actual values are optional.

---

# Question 8
## Searching in Unsorted Arrays

### Question
Searching is not possible in unsorted arrays.

## Correct Answer
✅ False

## Explanation

Linear Search works on unsorted arrays.

---

# Question 9
## Ordering Elements

### Question
The operation of ordering elements is called ______.

## Correct Answer
✅ Sorting

## Explanation

```text
5, 3, 1 -> 1, 3, 5
```

Ordering elements is called sorting.

---

# Question 10
## Random Access

### Question
Random access is not possible in arrays.

## Correct Answer
✅ False

## Explanation

```text
arr[3]
```

Direct access using index is possible.

---

# Question 11
## Locating Elements

### Question
______ is used to locate elements in arrays.

## Correct Answer
✅ Index

## Explanation

```text
arr[2]
```

`2` is the index.

---

# Question 12
## Valid Assignments

### Question

```text
numbers[10]
```

Which assignments are valid?

### Options
- a. numbers[9] <- 5
- b. numbers[10] <- 11
- c. numbers[11] <- 6
- d. numbers[0] <- 10

## Correct Answers
✅ a and d

## Explanation

Valid indices:

```text
0 to 9
```

---

# Question 13
## Correct Statement about Arrays

### Options
- ascending by default
- descending by default
- arranged contiguously

## Correct Answer
✅ arranged contiguously

## Explanation

Array elements are stored continuously in memory.

---

# Question 14
## Expression inside []

### Question
Expression within `[]` should resolve to a ______.

## Correct Answer
✅ positive number

## Explanation

```text
arr[0]
arr[5]
```

Indices should be non-negative integers.

---

# Question 15
## Heterogeneous Data

### Question
Can laptop details be stored in one normal array?

## Correct Answer
✅ No

## Explanation

Arrays store only same datatype.

---

# Question 16
## Songs List Example

### Question
List of songs in mobile phone is example of ______.

## Correct Answer
✅ Single-dimensional array

## Explanation

```text
songs[0]
songs[1]
```

Only one index required.

---

# Question 17
## Comparing Phone Prices

### Question
Comparing phone prices across shopping sites uses which array?

## Correct Answer
✅ Two-dimensional array

## Explanation

```text
           Amazon  Flipkart
Samsung    20000   19800
Redmi      15000   14900
```

Rows and columns form 2D array.

---

# Question 18
## Traversing Arrays

### Question
Arrays can only be traversed from first to last.

## Correct Answer
✅ False

## Explanation

Traversal possible:
- forward
- backward

---

# Question 19
## Rows and Columns

### Question
An array with rows and columns is called ______.

## Correct Answer
✅ Two-dimensional array

## Explanation

```text
matrix[3][4]
```

Rows + columns form 2D array.

---

# Question 20
## Correct Pseudocode

## Correct Answer
✅ Option d

```text
BEGIN
DECLARE name[20]
INPUT name
PRINT name
END
```

## Explanation

Correct order:
1. Declare array
2. Input values
3. Print values
