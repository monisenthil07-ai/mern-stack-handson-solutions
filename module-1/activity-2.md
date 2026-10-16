# Activity 2: Logic Building Challenge Students solve progressively complex logical problems using flowcharts and pseudocode before implementing them in code.
## Activity 2: Logic Building Challenge

**Aim:** To develop logical thinking and problem-solving skills by using pseudocode and flowcharts before implementing solutions in a programming language.

### Problem 1: Check Whether a Number Is Even or Odd

**Pseudocode:**

1. START
2. INPUT number
3. IF number MOD 2 = 0, PRINT "Even Number"
4. ELSE, PRINT "Odd Number"
5. STOP

**Flowchart:**

```text
       START
         |
         v
    Input Number
         |
         v
   Number % 2 == 0?
      /       \
    Yes        No
     |          |
     v          v
 Print Even  Print Odd
      \        /
         v
        STOP
```

**Python Program:**

```python
num = int(input("Enter a number: "))

if num % 2 == 0:
    print("Even Number")
else:
    print("Odd Number")
```

**Example Output:**

```text
Enter a number: 8
Even Number
```

### Problem 2: Find the Largest of Three Numbers

**Pseudocode:**

1. START
2. INPUT A, B, C
3. IF A >= B AND A >= C, PRINT A
4. ELSE IF B >= A AND B >= C, PRINT B
5. ELSE, PRINT C
6. STOP

**Python Program:**

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))

if a >= b and a >= c:
    print("Largest number:", a)
elif b >= a and b >= c:
    print("Largest number:", b)
else:
    print("Largest number:", c)
```

**Example Output:**

```text
Enter first number: 10
Enter second number: 25
Enter third number: 15
Largest number: 25
```

### Problem 3: Calculate the Sum of Numbers from 1 to N

**Pseudocode:**

1. START
2. INPUT N
3. SET SUM = 0
4. FOR I = 1 TO N
5. ```
   SUM = SUM + I
   ```
6. END FOR
7. PRINT SUM
8. STOP

**Python Program:**

```python
n = int(input("Enter a number: "))
total = 0

for i in range(1, n + 1):
    total += i

print("Sum =", total)
```

**Example Output:**

```text
Enter a number: 5
Sum = 15
```

### Result

The logical problems were solved using pseudocode and implemented in Python. This activity demonstrates how flowcharts and algorithms help convert real-world problems into executable programs.
