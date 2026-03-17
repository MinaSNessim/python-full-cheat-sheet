## functions

### lambda

You don't have to define the parameter inside lambda
```python
square = lambda x: x * x
result = square(5)
```

### recursive

```python
def factorial(n):
    if n == 1:
        return 1
    return n * factorial(n - 1)
    
print(factorial(5))
```

### important built in functions

#### breakpoint

The Python breakpoint() function is used to pause the program and start the debugger. We use it to inspect variables and code flow while debugging.

```python
Example:
# breakpoint() - Start debugger
x = 10
breakpoint()
print("Value of x is:", x)  # Output: Value of x is: 10 (after debugging)
```

#### classmethod

```python
class Demo:
    count = 0

    @classmethod
    def show_count(cls):
        print("Count is:", cls.count)

Demo.show_count()

Count is 0
```
