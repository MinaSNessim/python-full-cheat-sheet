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

#### delattr
```python
class MyClass:
    x = 10

delattr(MyClass, 'x')
print(MyClass.x)

AttributeError: type object 'MyClass' has no attribute 'x'
```

#### eval
```python
# eval() - Evaluate an expression
print("Eval result:", eval('3 + 5'))

8
```

#### format
```python
# format() - Format a value
formatted = "{:,.2f}".format(1234567.891)
print("Formatted number:", formatted) 

Formatted number: 1,234,567.89
```

#### filter
```python
nums = [1, 2, 3, 4, 5, 6]
even = filter(lambda x: x % 2 == 0, nums)
print("Even numbers:", list(even))

Even numbers: [2, 4, 6]
```

#### getattr
```python
# getattr() - Get attribute value from object
class Person:
    name = "Alice"
print("Name:", getattr(Person, 'name'))

Alice
```

#### help
```python
# help() - Show help on len() function
help(len)
Help on built-in function len in module builtins:

len(obj, /)
```

#### map
```python
# map() - Apply function to each item of iterable
mapped = list(map(lambda x: x * 2, [1, 2, 3]))
print("Mapped list:", mapped) 

Mapped list: [2, 4, 6]
```

#### zip
```python
# zip() - Combine iterables into tuples
print("Zipped lists:", list(zip(['a', 'b'], [1, 2]))) 

[('a', 1), ('b', 2)]
```












