## Reserved words

```python
import keyword
print(keyword.kwlist)

['False', 'None', 'True', 'and', 'as', 'assert', 'async', 'await', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']
```


### True, False
In Python, True and False are special keywords used to represent boolean values. We use them in conditions to check whether something is correct (True) or not (False) and control the program flow.

```python
Example:
x = 5
y = 3

print(x > y)   # True
print(x < y)   # False
Run Code

Output:
> True
> False
```

### None 
In Python, None means no value or nothing. It’s used when a variable is declared but not assigned any data. It helps to show that something is empty or not available yet.

```python
Example:
data = None

if data is None:
    print("No data found.")
else:
    print("Data is present.")
Run Code

Output:
No data found.
```

### and, or, not
And, or, and not are logical operators in Python and among the most important keywords of Python. The ‘and’ operator returns True if both operands are True. Here is the truth table for ‘and’:

```python
Example:
# Using and, or, and not

x = True
y = False

print("x and y:", x and y)   # False, because both are not True
print("x or y:", x or y)     # True, because one is True
print("not x:", not x)       # False, because x is True
Run Code

Output:
x and y: False
x or y: True
not x: False
```

### is 
The is keyword in Python checks whether two variables point to the same object in memory. It compares identity, not just value. Among the important Python keywords, is helps us compare object references, especially with None or singleton values.

```python
Example:
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)  # True
print(a is c)  # False
Run Code

Output:
True 
False
```

### in 
The in keyword is used to check if a value exists within a list, string, tuple, or other collections. It helps us know if something is present or not in a group of items.

```python
Example:
fruits = ["apple", "banana", "mango"]

print("apple" in fruits)   # True
print("grape" in fruits)   # False
Run Code

Output:
True
False
```

### if, else, and elif 
if, else, and elif are Python keywords used for decision-making. We use these control statements to execute code based on specific conditions:

if checks a condition, and if it’s true, its block runs.

elif (short for else if) checks another condition if the first is false.

else runs if none of the above conditions are true.

```python
Example:
score = 75

if score > 90:
    print("Excellent")
elif score > 60:
    print("Good")
else:
    print("Needs Improvement")
Run Code

Output:
Good
```

### del 
The Python del keyword deletes a reference to an object. We can delete any variable or list value using this keyword. You must know that everything is an object in Python. 

```python
Example:
numbers = [10, 20, 30, 40]
del numbers[2]

print(numbers)
Run Code

Output:
[10, 20, 40]
```

### for, while 
-for Keyword
The for keyword allows us to loop through a sequence like a list, string, or range. We use it to repeat actions for each item in a collection.

```python
Example:
for i in range(3):
    print("Hello", i)
Run Code

Output:

Hello 0
Hello 1
Hello 2
```

-while Keyword
The while keyword runs a block of code as long as a given condition is true. It’s useful when we don’t know how many times to loop.

```python
Example:
count = 0
while count < 3:
    print("Hi", count)
    count += 1
Run Code

Output:

Hi 0
Hi 1
Hi 2
```

### break, continue 
-break Keyword
The break keyword in Python is used to exit a loop immediately when a specific condition is true. We use it to stop further iterations once our task is done.

```python
Example:
for i in range(5):
    if i == 3:
        break
    print(i)
Run Code

Output:

0  
1  
3  
4
```

-Continue Keyword
The continue keyword skips the current loop iteration and moves to the next one. It’s helpful when we want to skip specific values or conditions without stopping the whole loop.

```python
Example:
for i in range(5):
    if i == 2:
        continue
    print(i)
Run Code

Output:

0  
1  
3  
4
Run Code
```

### import, from 
-import Keyword
The import keyword is used to bring an entire module into your program. It allows us to use functions, classes, or variables defined in that module.

```python
Example:

import math
print(math.sqrt(25))
Run Code

Output:

5.0
```

-from Keyword
The from keyword allows us to import specific parts of a module, like just one function or class.

```python
Example:

from math import sqrt
print(sqrt(36))
Run Code

Output:

6.0
```

### def 
The def keyword is used to define a function in Python. A function groups reusable code that runs when we call it using its name.

```python
Example:
def say_hello():
    print("hello there! have a good day")
   
say_hello() 
Run Code

Output:
hello there! have a good day
```

### as 
The as keyword is used to create an alias for the imported module. It gives a new name to the module while importing it. 

```python
Example:
import time as t  # aliasing time module as 't'

print("1")
t.sleep(5)
print("2")
Run Code

Output:
1
2
```

Note: The second line (2) appears after a 5-second delay because t.sleep(5) pauses the program for 5 seconds.

### With 
The with keyword in Python is used for managing resources like files. It needs a proper setup. Among important Python keywords, with simplifies code and automatically closes resources after use, even if an error occurs.

```python
Example:
with open("sample.txt", "w") as file:
    file.write("Hello, Python!")
Run Code

Then read the file:

with open("sample.txt", "r") as file:
    print(file.read())

Output:
Hello, Python!
```

### class 
The class keyword declares user-defined classes in Python. Classes are a collection of related methods and attributes representing a real-world situation. Although they can be defined anywhere in a program, it is recommended to define a single class in a module. 

The idea of bringing functions and data together in a class is the core of object-oriented programming (OOP). 

```python
Example:
class MyClass:
    pass

my_instance = MyClass()
print(type(my_instance))
Run Code

Output:
<class '__main__.MyClass'>
```

### pass 
In Python, the pass keyword is a null statement. When we execute the pass keyword, it produces no output. Pass is used as a placeholder and prevents indentation errors. 

```python
Example:
# Define a simple class
class MyClass:
    pass
# Create an instance of the class
my_instance = MyClass()

(No output, as nothing is defined inside the class)
```

### lambda 
lambda creates an anonymous function, which means a function with no name. It is used to make an inline returning function with no return statement allowed internally. This keyword consists of expressions that are evaluated and returned. 

```python
Example:
# Define a lambda function that adds two numbers
add = lambda x, y: x + y
# Use the lambda function
result = add(2, 3)
print(result)  
Run Code

Output:
5
```

### try, raise, except 
Exceptions are errors suggesting there is something wrong while executing the program. A few common examples of exceptions in Python are ImportError, IOError, NameError, ValueError, TypeError, and ZeroDivisionError. 

We use try—except blocks to catch exceptions. You can understand all keywords in Python better through the given examples.

try: This keyword is used to catch errors in code. Once the code in the try block is checked and an error is found, the except block is executed.

raise: Using the raise keyword, we can raise an explicit exception.

except: This keyword is used with ‘try’ to catch exceptions.

```python
Example:
# Example using try, except, and raise

def divide(x, y):
    try:
        if y == 0:
            raise ZeroDivisionError("You can't divide by zero!")
        result = x / y
    except ZeroDivisionError as e:
        print("Error:", e)
    else:
        print("Result:", result)

divide(10, 0)
Run Code

Output:
Error: You can't divide by zero!
```

### finally, assert 
-finally Keyword
The finally block in Python always runs after try and except, whether an error occurred or not.

```python
Example:

try:
    print("Trying...")
    x = 1 / 0
except ZeroDivisionError:
    print("Caught an error")
finally:
    print("This always runs")
Run Code

Output:

Trying...
Caught an error
This always runs
```

-assert Keyword
The assert keyword checks if a condition is true. If not, it stops the program and shows an error. It’s useful for debugging.

```python
Example:

age = 18
assert age >= 18
print("Access granted")
Run Code

Output:

Access granted
```

### return 
We use the return keyword to return a final result from a function. It is used within a function and exits it immediately while returning a value. If a value is not returned explicitly, it returns None automatically. 

```python
Example:
def add(a, b):
    return a + b

result = add(3, 5)
print("Sum:", result)
Run Code

Output:
Sum: 8
```

### yield 
yield is used like a return statement inside a function. It returns a generator, which is an iterator that generates one item at a time. As a long list of values can consume a lot of memory, we use generators to generate one value at a time rather than storing all the values together. 

The return keyword returns a single value and ends the function, whereas the yield keyword returns multiple values, but one at a time.

```python
Example:
def even_numbers(n):
    for i in range(n):
        if i % 2 == 0:
            yield i

# Using the generator
for num in even_numbers(6):
    print(num)
Run Code

Output:
0
2
4
```

### async, await 
In Python, the asyncio library provides async and await keywords. They both are used to write concurrent code in Python. We use async to define asynchronous functions and await to pause execution until the awaited task completes.

```python
Example:
import asyncio

async def fetch_data():
    print("Start fetching")
    await asyncio.sleep(2)
    print("Done fetching")

asyncio.run(fetch_data())
Run Code

Output:
Start fetching
Done fetching
```

### global
When we need to change the value of a global variable inside a function, we must declare it using the global keyword. If we don’t use this keyword, it will create a local variable with that name. However, if we have to read the value of a global variable, we don’t have to define it as global. 

```python
example:
x = 10  # Global variable

def modify_global():
    global x  # Declare x as global
    x = 20    # Modify the global variable
    print(f"Inside modify_global: x = {x}")

modify_global()
print(f"Outside modify_global: x = {x}")
Run Code

Output:
Inside modify_global: x = 20
Outside modify_global: x = 20
```

### nonlocal
The nonlocal keyword in Python is used to modify a variable in the nearest enclosing (non-global) scope. Among important Python keywords, it helps us update variables inside nested functions without making them global.

```python
Example:
def outer():
    x = 5
    def inner():
        nonlocal x
        x = 10
        print("Inner:", x)
    inner()
    print("Outer:", x)

outer()
Run Code

Output:
Inner: 10
Outer: 10
```
