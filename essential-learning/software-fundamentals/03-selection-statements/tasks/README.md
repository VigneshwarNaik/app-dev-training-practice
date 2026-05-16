# Pseudocode Using Selection Statements

This repository contains pseudocode programs using:
- `IF`
- `ELSE IF`
- `AND`
- `OR`
- Nested IF conditions

These tasks are useful for beginners learning selection statements and decision-making logic.

---

# 1. Work Allotment

## Problem Statement
To decide on an employee's work allotment, the manager asks for:
- Age
- Sex (M/F)
- Marital Status (Y/N)

### Rules
- Female employees work only in urban areas.
- Male unmarried employees aged 20–40 can work anywhere.
- Male unmarried employees aged 41–60 work in urban areas.
- Married male employees work in urban areas.

### Special Conditions
- If age < 20 → `"Age limit is less"`
- If age > 60 → `"Age limit is high"`
- If age < 0 → `"Invalid age"`

---

## Explanation
1. Check invalid age conditions.
2. Check whether employee is male or female.
3. Apply work allotment rules using nested IF statements.

---

## Pseudocode

```text
BEGIN

INPUT age
INPUT sex
INPUT marital_status

IF age < 0 THEN
    PRINT "Invalid age"

ELSE IF age < 20 THEN
    PRINT "Age limit is less"

ELSE IF age > 60 THEN
    PRINT "Age limit is high"

ELSE

    IF sex = "F" THEN
        PRINT "She will work in urban areas only"

    ELSE

        IF marital_status = "Y" THEN
            PRINT "He will work in urban areas"

        ELSE

            IF age >= 20 AND age <= 40 THEN
                PRINT "He could be put to work anywhere"

            ELSE
                PRINT "He will work in urban areas"

            END IF

        END IF

    END IF

END IF

END
```

---

# 2. Highways-Department Celebration

## Problem Statement
At a toll gate:
- Vehicle number divisible by both 3 and 5 → Free
- Divisible by either 3 or 5 → Half fee
- Otherwise → Full fee

Use:
- `AND`
- `OR`
- Else-if ladder

---

## Explanation
- Use `MOD` operator to check divisibility.
- Check:
  1. Both divisible
  2. Either divisible
  3. Otherwise

---

## Pseudocode

```text
BEGIN

INPUT vehicle_number

IF vehicle_number MOD 3 = 0 AND vehicle_number MOD 5 = 0 THEN
    PRINT "Vehicle can move for free of cost"

ELSE IF vehicle_number MOD 3 = 0 OR vehicle_number MOD 5 = 0 THEN
    PRINT "Pay half of the fee"

ELSE
    PRINT "Pay full amount"

END IF

END
```

---

# 3. Names of the Month

## Problem Statement
Nancy teaches seasons using month names.

### Seasons
- Summer → March, April, May
- Winter → December, January, February
- Autumn → September, October, November
- Spring → June, July, August

---

## Explanation
- Input month name.
- Use OR condition to check season.

---

## Pseudocode

```text
BEGIN

INPUT month

IF month = "March" OR month = "April" OR month = "May" THEN
    PRINT "Summer"

ELSE IF month = "December" OR month = "January" OR month = "February" THEN
    PRINT "Winter"

ELSE IF month = "September" OR month = "October" OR month = "November" THEN
    PRINT "Autumn"

ELSE IF month = "June" OR month = "July" OR month = "August" THEN
    PRINT "Spring"

ELSE
    PRINT "Invalid Month"

END IF

END
```

---

# 4. Income Tax Calculation

## Problem Statement
Calculate income tax based on:
- Age
- Income

### Special Conditions
- Age < 20 → `"Age is less"`
- Age > 100 OR age < 0 OR income < 0 → `"Invalid input"`

---

## Tax Slabs

### Age 20–59
| Income Range | Tax |
|---|---|
| ≤ 2,50,000 | 0% |
| 2,50,001 – 5,00,000 | 10% |
| 5,00,001 – 10,00,000 | 20% |
| > 10,00,000 | 30% |

### Age 60–80
| Income Range | Tax |
|---|---|
| ≤ 3,00,000 | 0% |
| 3,00,001 – 5,00,000 | 10% |
| 5,00,001 – 10,00,000 | 20% |
| > 10,00,000 | 30% |

### Age 81–100
| Income Range | Tax |
|---|---|
| ≤ 5,00,000 | 0% |
| 5,00,001 – 10,00,000 | 20% |
| > 10,00,000 | 30% |

---

## Explanation
1. Validate age and income.
2. Identify age group.
3. Apply tax slab conditions.

---

## Pseudocode

```text
BEGIN

INPUT age
INPUT income

IF age < 20 AND age >= 0 THEN
    PRINT "Age is less"

ELSE IF age > 100 OR age < 0 OR income < 0 THEN
    PRINT "Invalid input"

ELSE IF age >= 20 AND age < 60 THEN

    IF income <= 250000 THEN
        PRINT "0% tax"

    ELSE IF income <= 500000 THEN
        PRINT "10% tax"

    ELSE IF income <= 1000000 THEN
        PRINT "20% tax"

    ELSE
        PRINT "30% tax"

    END IF

ELSE IF age >= 60 AND age <= 80 THEN

    IF income <= 300000 THEN
        PRINT "0% tax"

    ELSE IF income <= 500000 THEN
        PRINT "10% tax"

    ELSE IF income <= 1000000 THEN
        PRINT "20% tax"

    ELSE
        PRINT "30% tax"

    END IF

ELSE

    IF income <= 500000 THEN
        PRINT "0% tax"

    ELSE IF income <= 1000000 THEN
        PRINT "20% tax"

    ELSE
        PRINT "30% tax"

    END IF

END IF

END
```

---

# 5. Land Mark Store

## Problem Statement
Annie wants to reach floor `n`.

The lift stops only at:
- n1
- n2
- n3

She should get down at the nearest floor.

If two floors are equally near:
- She prefers walking down instead of climbing up.

If any floor number is negative:
- `"Invalid Floor number"`

---

## Explanation
1. Check invalid floor numbers.
2. Calculate distance from target floor.
3. Choose nearest floor.
4. If distances are equal:
   - Prefer higher floor.

---

## Example

### Input
```text
Target Floor = 10
Lift Stops = 8, 4, 15
```

### Output
```text
You may get down at floor number 8
```

---

## Pseudocode

```text
BEGIN

INPUT n
INPUT n1
INPUT n2
INPUT n3

IF n < 0 OR n1 < 0 OR n2 < 0 OR n3 < 0 THEN
    PRINT "Invalid Floor number"

ELSE

    d1 = ABS(n - n1)
    d2 = ABS(n - n2)
    d3 = ABS(n - n3)

    min = d1
    floor = n1

    IF d2 < min OR (d2 = min AND n2 > floor) THEN
        min = d2
        floor = n2
    END IF

    IF d3 < min OR (d3 = min AND n3 > floor) THEN
        min = d3
        floor = n3
    END IF

    PRINT "You may get down at floor number", floor

END IF

END
```

---

# Conclusion

These pseudocode programs demonstrate:
- Decision-making statements
- Nested IF logic
- Else-if ladder
- AND / OR operators
- Real-world problem solving using pseudocode

They are useful for:
- Beginners
- College lab programs
- Interview preparation
- Programming fundamentals practice
