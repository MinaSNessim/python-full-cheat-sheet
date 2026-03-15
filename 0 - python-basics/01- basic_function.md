## print()
The Python print command allows us to control how we display output using different parameters. These make our code clearer and more flexible.

objects: The values we want to print. It can be text, numbers, lists, or any object.

sep: Sets the separator between printed items. By default, it’s a space, but we can change it.

end: Tells what to print at the end. By default, it's a newline (\n), but we can change it.

file: Defines where to send the output. By default, it prints to the screen (sys.stdout).

flush: If set to True, it forces the output to appear immediately without waiting or buffering.


```python
print(object(s), sep='separator', end='end', file=file, flush=flush)

print("Welcome", "to", "WsCube Tech", sep="-", end="!\n")
```

### print concatenate 

```python
part1 = "Welcome to "
part2 = "WsCube Tech"
print(part1 + part2)
```

### unpacking a list

```python
numbers = [1, 2, 3, 4]
print(*numbers, sep=", ")
```

## comments 

```python
# single line comment
'''
multi line
comments
'''
```

## variables rules

Rules for Python Variables
1. Python variables must start with a letter or an underscore (e.g., _name, age).
2.We can not start variable names with a number.
3. Use only letters, numbers, and underscores (no spaces or special characters).
4. Don’t use Python keywords like if, class, or while as variable names.
5. Variable names are case-sensitive (Age and age are different).
6. Choose names that make sense (like total_price, not tp).

## Object Reference in Python

```python
Example:
a = [1, 2, 3]    # 'a' refers to a list object
b = a            # 'b' now refers to the same list object
b.append(4)      # modifying the list through 'b'
print(a)
Run Code

Output:
[1, 2, 3, 4]
```

