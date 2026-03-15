## mathematical operations

```python
x = 10
y = 3

# Addition
print(x + y)   
13
# Subtraction
print(x - y)   
7
# Multiplication
print(x * y)   
30
# Division
print(x / y)   
3.3333333333333335
# Floor Division
print(x // y)  
3
# Modulus
print(x % y)   
1
# Exponentiation
print(x ** y)  
1000
```

## order of operations

P E M D A S
1- P – Parentheses ()
2- E – Exponentiation **
3- M – Multiplication *
4- D – Division / (same precedence as *, //, %)
5- A – Addition +
6- S – Subtraction -

## comparison operations


```python 
x = 10
y = 5

# Greater than
print(x > y)   
True

# Less than
print(x < y)   
False

# Greater than or equal to
print(x >= y)  
True

# Less than or equal to
print(x <= y)  
False

# Equal to
print(x == y)  
False

# Not equal to
print(x != y) 
True
```

## assignment operators

```python
x = 10
y = 3

x = y + 2
print("x = y + 2:", x)  
x = y + 2: 5

# Addition Assignment
x += y  # x = x + y
print("x += y:", x)     
x += y: 8

# Subtraction Assignment
x -= y  # x = x - y
print("x -= y:", x)     
x -= y: 5

# Multiplication Assignment
x *= y  # x = x * y
print("x *= y:", x)     
x *= y: 15

# Division Assignment
x /= y  # x = x / y
print("x /= y:", x)     
x /= y: 5.0

# Remainder Assignment
x %= y  # x = x % y
print("x %= y:", x)     
x %= y: 2.0

# Floor Division Assignment
x //= y  # x = x // y
print("x //= y:", x)    
x //= y: 0.0

# Exponent Assignment
x **= y  # x = x ** y
print("x **= y:", x)
x **= y: 0.0
```

## logical operators

```python
x = True
y = False

# Logical AND
print("x and y:", x and y)  
x and y: False

# Logical OR
print("x or y:", x or y)     
x or y: True

# Logical NOT
print("not x:", not x)
not x: False
print("not y:", not y)
not y: True
```

## bitwise operators

```python
x = 6   # binary: 110
y = 3   # binary: 011

# Bitwise AND Sets each bit to 1 if both bits at the same position are 1.
print("x & y:", x & y)   
x & y: 2

# Bitwise OR Sets each bit to 1 if at least one bit at that position is 1.
print("x | y:", x | y)   
x | y: 7

# Bitwise XOR Sets each bit to 1 if the corresponding bits are different.
print("x ^ y:", x ^ y)   
x ^ y: 5

# Bitwise NOT Inverts all the bits: 0 becomes 1, and 1 becomes 0.
print("~x:", ~x)        
~x: -7

# Bitwise Right Shift Shifts the bits to the right by a specified number of positions.
print("x >> 1:", x >> 1) 
x >> 1: 3

# Bitwise Left Shift Shifts the bits to the left and fills the rightmost bits with zeros.
print("x << 1:", x << 1)
x << 1: 12
```
