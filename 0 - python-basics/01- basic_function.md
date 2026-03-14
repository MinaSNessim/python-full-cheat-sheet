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
