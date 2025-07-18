# Python Operators Study Guide

## Table of Contents
1. [Arithmetic Operators](#arithmetic-operators)
2. [Comparison Operators](#comparison-operators)
3. [Logical Operators](#logical-operators)
4. [Assignment Operators](#assignment-operators)
5. [Bitwise Operators](#bitwise-operators)
6. [Identity Operators](#identity-operators)
7. [Membership Operators](#membership-operators)
8. [Operator Precedence](#operator-precedence)
9. [Practice Examples](#practice-examples)

---

## Arithmetic Operators

Arithmetic operators perform mathematical operations on numbers.

| Operator | Name | Example | Result |
|----------|------|---------|--------|
| `+` | Addition | `5 + 3` | `8` |
| `-` | Subtraction | `5 - 3` | `2` |
| `*` | Multiplication | `5 * 3` | `15` |
| `/` | Division | `10 / 3` | `3.333...` |
| `//` | Floor Division | `10 // 3` | `3` |
| `%` | Modulus | `10 % 3` | `1` |
| `**` | Exponentiation | `2 ** 3` | `8` |

### Examples:
```python
# Basic arithmetic
a = 10
b = 3

print(a + b)    # 13
print(a - b)    # 7
print(a * b)    # 30
print(a / b)    # 3.3333333333333335
print(a // b)   # 3 (floor division)
print(a % b)    # 1 (remainder)
print(a ** b)   # 1000 (10 to the power of 3)
```

---

## Comparison Operators

Comparison operators compare two values and return a boolean result.

| Operator | Name | Example | Result |
|----------|------|---------|--------|
| `==` | Equal to | `5 == 5` | `True` |
| `!=` | Not equal to | `5 != 3` | `True` |
| `>` | Greater than | `5 > 3` | `True` |
| `<` | Less than | `5 < 3` | `False` |
| `>=` | Greater than or equal | `5 >= 5` | `True` |
| `<=` | Less than or equal | `3 <= 5` | `True` |

### Examples:
```python
x = 10
y = 5

print(x == y)   # False
print(x != y)   # True
print(x > y)    # True
print(x < y)    # False
print(x >= 10)  # True
print(y <= 5)   # True
```

---

## Logical Operators

Logical operators combine boolean values or expressions.

| Operator | Description | Example | Result |
|----------|-------------|---------|--------|
| `and` | Returns True if both operands are True | `True and False` | `False` |
| `or` | Returns True if at least one operand is True | `True or False` | `True` |
| `not` | Returns the opposite boolean value | `not True` | `False` |

### Truth Tables:

**AND Operator:**
- `True and True` = `True`
- `True and False` = `False`
- `False and True` = `False`
- `False and False` = `False`

**OR Operator:**
- `True or True` = `True`
- `True or False` = `True`
- `False or True` = `True`
- `False or False` = `False`

### Examples:
```python
a = True
b = False

print(a and b)      # False
print(a or b)       # True
print(not a)        # False
print(not b)        # True

# With conditions
x = 10
y = 5
print(x > 5 and y < 10)  # True
print(x < 5 or y > 3)    # True
```

---

## Assignment Operators

Assignment operators assign values to variables.

| Operator | Example | Equivalent to |
|----------|---------|---------------|
| `=` | `x = 5` | `x = 5` |
| `+=` | `x += 3` | `x = x + 3` |
| `-=` | `x -= 3` | `x = x - 3` |
| `*=` | `x *= 3` | `x = x * 3` |
| `/=` | `x /= 3` | `x = x / 3` |
| `//=` | `x //= 3` | `x = x // 3` |
| `%=` | `x %= 3` | `x = x % 3` |
| `**=` | `x **= 3` | `x = x ** 3` |

### Examples:
```python
x = 10

x += 5      # x = 15
x -= 3      # x = 12
x *= 2      # x = 24
x /= 4      # x = 6.0
x //= 2     # x = 3.0
x %= 2      # x = 1.0
x **= 3     # x = 1.0
```

---

## Bitwise Operators

Bitwise operators work on bits and perform bit-by-bit operations.

| Operator | Name | Example | Result |
|----------|------|---------|--------|
| `&` | AND | `5 & 3` | `1` |
| `|` | OR | `5 | 3` | `7` |
| `^` | XOR | `5 ^ 3` | `6` |
| `~` | NOT | `~5` | `-6` |
| `<<` | Left Shift | `5 << 2` | `20` |
| `>>` | Right Shift | `5 >> 1` | `2` |

### Examples:
```python
a = 5   # Binary: 101
b = 3   # Binary: 011

print(a & b)    # 1 (Binary: 001)
print(a | b)    # 7 (Binary: 111)
print(a ^ b)    # 6 (Binary: 110)
print(~a)       # -6
print(a << 2)   # 20 (Binary: 10100)
print(a >> 1)   # 2 (Binary: 10)
```

---

## Identity Operators

Identity operators compare the memory location of two objects.

| Operator | Description | Example |
|----------|-------------|---------|
| `is` | Returns True if both variables point to the same object | `x is y` |
| `is not` | Returns True if variables point to different objects | `x is not y` |

### Examples:
```python
x = [1, 2, 3]
y = [1, 2, 3]
z = x

print(x == y)       # True (same content)
print(x is y)       # False (different objects)
print(x is z)       # True (same object)
print(x is not y)   # True
```

---

## Membership Operators

Membership operators test if a value is present in a sequence.

| Operator | Description | Example |
|----------|-------------|---------|
| `in` | Returns True if value is found in sequence | `'a' in 'apple'` |
| `not in` | Returns True if value is not found in sequence | `'z' not in 'apple'` |

### Examples:
```python
# With strings
text = "Hello World"
print('H' in text)          # True
print('z' not in text)      # True

# With lists
numbers = [1, 2, 3, 4, 5]
print(3 in numbers)         # True
print(6 not in numbers)     # True

# With dictionaries (checks keys)
person = {'name': 'John', 'age': 30}
print('name' in person)     # True
print('height' not in person)  # True
```

---

## Operator Precedence

Operators have different precedence levels. Higher precedence operators are evaluated first.

**From highest to lowest precedence:**

1. `()` - Parentheses
2. `**` - Exponentiation
3. `+x`, `-x`, `~x` - Unary plus, minus, bitwise NOT
4. `*`, `/`, `//`, `%` - Multiplication, division, floor division, modulus
5. `+`, `-` - Addition, subtraction
6. `<<`, `>>` - Bitwise shifts
7. `&` - Bitwise AND
8. `^` - Bitwise XOR
9. `|` - Bitwise OR
10. `==`, `!=`, `<`, `<=`, `>`, `>=`, `is`, `is not`, `in`, `not in` - Comparisons
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
```

---

## Practice Examples

### Example 1: Calculator
```python
def calculator(a, b, operator):
    if operator == '+':
        return a + b
    elif operator == '-':
        return a - b
    elif operator == '*':
        return a * b
    elif operator == '/':
        return a / b if b != 0 else "Cannot divide by zero"
    elif operator == '**':
        return a ** b
    else:
        return "Invalid operator"

print(calculator(10, 3, '+'))   # 13
print(calculator(10, 3, '/'))   # 3.333...
```

### Example 2: Boolean Logic
```python
def check_eligibility(age, has_license, has_insurance):
    can_drive = age >= 18 and has_license and has_insurance
    return can_drive

print(check_eligibility(20, True, True))   # True
print(check_eligibility(16, True, True))   # False
```

### Example 3: Working with Lists
```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Find even numbers
even_numbers = [num for num in numbers if num % 2 == 0]
print(even_numbers)  # [2, 4, 6, 8, 10]

# Check if number exists
target = 7
if target in numbers:
    print(f"{target} is in the list")
else:
    print(f"{target} is not in the list")
```

### Example 4: String Operations
```python
text = "Python Programming"

# Check if substring exists
if "Python" in text:
    print("Found Python!")

# Count vowels
vowels = "aeiouAEIOU"
vowel_count = sum(1 for char in text if char in vowels)
print(f"Vowels: {vowel_count}")
```

---

## Quick Reference Cheat Sheet

```python
# Arithmetic: +, -, *, /, //, %, **
# Comparison: ==, !=, <, >, <=, >=
# Logical: and, or, not
# Assignment: =, +=, -=, *=, /=, //=, %=, **=
# Bitwise: &, |, ^, ~, <<, >>
# Identity: is, is not
# Membership: in, not in
```

## Tips for Learning:
1. Practice with interactive Python shell
2. Start with simple examples and gradually increase complexity
3. Pay attention to operator precedence
4. Use parentheses when in doubt about precedence
5. Remember that comparison operators return boolean values
6. Understand the difference between `==` (equality) and `is` (identity)
7. Practice with different data types (numbers, strings, lists, etc.)

Happy coding! 🐍
