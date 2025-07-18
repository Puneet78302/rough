# Python Operators Study Guide

## Overview
Operators are special symbols that perform operations on variables and values. Python supports various types of operators that allow you to manipulate data and perform calculations.

## 1. Arithmetic Operators

Arithmetic operators perform mathematical operations on numeric values.

| Operator | Name | Description | Example | Result |
|----------|------|-------------|---------|--------|
| `+` | Addition | Adds two operands | `5 + 3` | `8` |
| `-` | Subtraction | Subtracts right operand from left | `5 - 3` | `2` |
| `*` | Multiplication | Multiplies two operands | `5 * 3` | `15` |
| `/` | Division | Divides left operand by right | `10 / 3` | `3.3333...` |
| `//` | Floor Division | Returns floor of division | `10 // 3` | `3` |
| `%` | Modulus | Returns remainder of division | `10 % 3` | `1` |
| `**` | Exponentiation | Raises left operand to power of right | `2 ** 3` | `8` |

### Examples:
```python
a = 10
b = 3

print(a + b)    # 13
print(a - b)    # 7
print(a * b)    # 30
print(a / b)    # 3.3333333333333335
print(a // b)   # 3
print(a % b)    # 1
print(a ** b)   # 1000
```

## 2. Comparison Operators

Comparison operators compare two values and return a boolean result (True or False).

| Operator | Name | Description | Example | Result |
|----------|------|-------------|---------|--------|
| `==` | Equal | Checks if values are equal | `5 == 5` | `True` |
| `!=` | Not Equal | Checks if values are not equal | `5 != 3` | `True` |
| `>` | Greater Than | Checks if left > right | `5 > 3` | `True` |
| `<` | Less Than | Checks if left < right | `5 < 3` | `False` |
| `>=` | Greater Than or Equal | Checks if left >= right | `5 >= 5` | `True` |
| `<=` | Less Than or Equal | Checks if left <= right | `3 <= 5` | `True` |

### Examples:
```python
x = 10
y = 5

print(x == y)   # False
print(x != y)   # True
print(x > y)    # True
print(x < y)    # False
print(x >= y)   # True
print(x <= y)   # False
```

## 3. Logical Operators

Logical operators combine conditional statements.

| Operator | Description | Example | Result |
|----------|-------------|---------|--------|
| `and` | Returns True if both statements are true | `True and False` | `False` |
| `or` | Returns True if one statement is true | `True or False` | `True` |
| `not` | Reverses the result | `not True` | `False` |

### Examples:
```python
a = True
b = False

print(a and b)  # False
print(a or b)   # True
print(not a)    # False
print(not b)    # True

# Practical example
age = 25
has_license = True

can_drive = age >= 18 and has_license
print(can_drive)  # True
```

## 4. Assignment Operators

Assignment operators assign values to variables.

| Operator | Name | Description | Example | Equivalent |
|----------|------|-------------|---------|------------|
| `=` | Assignment | Assigns value | `x = 5` | `x = 5` |
| `+=` | Add and Assign | Adds and assigns | `x += 3` | `x = x + 3` |
| `-=` | Subtract and Assign | Subtracts and assigns | `x -= 3` | `x = x - 3` |
| `*=` | Multiply and Assign | Multiplies and assigns | `x *= 3` | `x = x * 3` |
| `/=` | Divide and Assign | Divides and assigns | `x /= 3` | `x = x / 3` |
| `//=` | Floor Divide and Assign | Floor divides and assigns | `x //= 3` | `x = x // 3` |
| `%=` | Modulus and Assign | Modulus and assigns | `x %= 3` | `x = x % 3` |
| `**=` | Exponent and Assign | Exponentiates and assigns | `x **= 3` | `x = x ** 3` |

### Examples:
```python
x = 10

x += 5   # x = x + 5 → x = 15
x -= 3   # x = x - 3 → x = 12
x *= 2   # x = x * 2 → x = 24
x /= 4   # x = x / 4 → x = 6.0
x //= 2  # x = x // 2 → x = 3.0
x %= 2   # x = x % 2 → x = 1.0
x **= 3  # x = x ** 3 → x = 1.0
```

## 5. Bitwise Operators

Bitwise operators work on bits and perform bit-by-bit operations.

| Operator | Name | Description | Example | Result |
|----------|------|-------------|---------|--------|
| `&` | AND | Sets bit to 1 if both bits are 1 | `5 & 3` | `1` |
| `\|` | OR | Sets bit to 1 if any bit is 1 | `5 \| 3` | `7` |
| `^` | XOR | Sets bit to 1 if bits are different | `5 ^ 3` | `6` |
| `~` | NOT | Inverts all bits | `~5` | `-6` |
| `<<` | Left Shift | Shifts bits left | `5 << 1` | `10` |
| `>>` | Right Shift | Shifts bits right | `5 >> 1` | `2` |

### Examples:
```python
a = 5   # Binary: 101
b = 3   # Binary: 011

print(a & b)   # 1 (Binary: 001)
print(a | b)   # 7 (Binary: 111)
print(a ^ b)   # 6 (Binary: 110)
print(~a)      # -6
print(a << 1)  # 10 (Binary: 1010)
print(a >> 1)  # 2 (Binary: 10)
```

## 6. Membership Operators

Membership operators test if a value is present in a sequence.

| Operator | Description | Example | Result |
|----------|-------------|---------|--------|
| `in` | Returns True if value is in sequence | `'a' in 'hello'` | `False` |
| `not in` | Returns True if value is not in sequence | `'a' not in 'hello'` | `True` |

### Examples:
```python
text = "Hello World"
numbers = [1, 2, 3, 4, 5]

print('H' in text)          # True
print('x' in text)          # False
print('x' not in text)      # True
print(3 in numbers)         # True
print(6 not in numbers)     # True
```

## 7. Identity Operators

Identity operators compare the memory location of two objects.

| Operator | Description | Example | Result |
|----------|-------------|---------|--------|
| `is` | Returns True if variables are the same object | `x is y` | Depends on objects |
| `is not` | Returns True if variables are different objects | `x is not y` | Depends on objects |

### Examples:
```python
x = [1, 2, 3]
y = [1, 2, 3]
z = x

print(x == y)       # True (same content)
print(x is y)       # False (different objects)
print(x is z)       # True (same object)
print(x is not y)   # True (different objects)

# With immutable objects
a = 5
b = 5
print(a is b)       # True (Python optimizes small integers)
```

## 8. Operator Precedence

Operators have different precedence levels. Higher precedence operators are evaluated first.

### Precedence Order (High to Low):
1. `()` - Parentheses
2. `**` - Exponentiation
3. `+x, -x, ~x` - Unary plus, minus, NOT
4. `*, /, //, %` - Multiplication, Division, Floor Division, Modulus
5. `+, -` - Addition, Subtraction
6. `<<, >>` - Bitwise shifts
7. `&` - Bitwise AND
8. `^` - Bitwise XOR
9. `|` - Bitwise OR
10. `==, !=, <, <=, >, >=, is, is not, in, not in` - Comparisons
11. `not` - Logical NOT
12. `and` - Logical AND
13. `or` - Logical OR

### Examples:
```python
# Without parentheses
result = 2 + 3 * 4      # 14 (not 20)
result = 2 ** 3 * 4     # 32 (not 4096)

# With parentheses
result = (2 + 3) * 4    # 20
result = 2 ** (3 * 4)   # 4096

# Complex expression
result = 10 + 5 * 2 - 3 / 3
# Evaluation: 10 + 10 - 1.0 = 19.0
```

## 9. Practical Examples

### Calculator Function
```python
def calculator(a, b, operation):
    if operation == '+':
        return a + b
    elif operation == '-':
        return a - b
    elif operation == '*':
        return a * b
    elif operation == '/':
        return a / b if b != 0 else "Cannot divide by zero"
    elif operation == '**':
        return a ** b
    else:
        return "Invalid operation"

print(calculator(10, 5, '+'))   # 15
print(calculator(10, 5, '*'))   # 50
print(calculator(10, 0, '/'))   # Cannot divide by zero
```

### Grade Evaluation
```python
def evaluate_grade(score):
    if score >= 90:
        return 'A'
    elif score >= 80:
        return 'B'
    elif score >= 70:
        return 'C'
    elif score >= 60:
        return 'D'
    else:
        return 'F'

# Using comparison operators
score = 85
grade = evaluate_grade(score)
print(f"Score: {score}, Grade: {grade}")  # Score: 85, Grade: B
```

### List Operations
```python
# Using membership and logical operators
fruits = ['apple', 'banana', 'orange', 'grape']
favorite_fruits = ['apple', 'grape']

for fruit in fruits:
    if fruit in favorite_fruits:
        print(f"{fruit} is a favorite!")
    else:
        print(f"{fruit} is not a favorite.")

# Using logical operators
has_apple = 'apple' in fruits
has_mango = 'mango' in fruits
print(f"Has apple and mango: {has_apple and has_mango}")  # False
print(f"Has apple or mango: {has_apple or has_mango}")    # True
```

## 10. Common Mistakes and Tips

### Mistake 1: Using `=` instead of `==`
```python
# Wrong
if x = 5:  # SyntaxError
    print("x is 5")

# Correct
if x == 5:
    print("x is 5")
```

### Mistake 2: Confusing `is` with `==`
```python
# Be careful with identity vs equality
list1 = [1, 2, 3]
list2 = [1, 2, 3]

print(list1 == list2)  # True (same content)
print(list1 is list2)  # False (different objects)
```

### Mistake 3: Division operator differences
```python
# Integer division vs float division
print(10 / 3)   # 3.3333333333333335 (float)
print(10 // 3)  # 3 (integer)
```

### Tips:
- Use parentheses to make operator precedence clear
- Remember that `//` gives integer division, `/` gives float division
- Use `is` for None comparisons: `if x is None:`
- Chain comparisons: `if 0 < x < 10:`
- Use augmented assignment operators for cleaner code

## Practice Exercises

1. Write a program that calculates the area of a circle using `**` operator
2. Create a function that checks if a number is even using the `%` operator
3. Use logical operators to validate user input (age between 18-65 and has valid ID)
4. Practice bitwise operations with binary number manipulation
5. Create a program that uses membership operators to check if words are in a sentence

## Summary

Python operators are essential tools for data manipulation and program logic. Understanding their precedence, proper usage, and common pitfalls will help you write more efficient and readable code. Practice using different operators in various contexts to master their application.