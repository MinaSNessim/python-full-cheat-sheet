## string methods

```python
upper() Converts the string to uppercase

lower() Converts the string to lowercase

capitalize() Capitalizes the first character of the string

partition() Splits string into a tuple at the first match of the separator.

replace() Replaces part of the string with another value

encode() Encodes string to bytes (UTF-8 by default)

find() Returns the index of the first occurrence of a substring

title() Converts string to title case (each word starts with a capital letter)

rstrip() Removes trailing whitespace or characters

split() Splits the string from left

startswith() Checks if a string begins with the specified string or not.

isnumeric() checks numeric characters

index() returns the index of a substring.
```

## lists methods

Ordered: Lists are ordered, which means they follow a specific order while adding data.
Mutable:  We can change, add, or remove elements after creating the list.
Allows Duplicates: We can store the same value more than once in a list.
Holds Different Data Types: We can store numbers, strings, or even other lists together.
Indexable: We access elements using their index, starting from 0.

```python
append() adds one element at a time without changing existing items.

insert() add an element at a specific index in the list. It shifts the existing elements to the right.

extend() add elements of another list to the current list.

remove() delete a specific item by its value. It only removes the first match found in the list.

pop() remove an element from the list and return it

del to remove an element from a list by its index
```

### list comprehension 

```python
newList = [ expression(element) for element in oldList if condition ]
li = [num for num in range(20) if num % 2 == 0]
print(li)
[0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
```


### more lists methods

```python
Count() Returns the number of times an item is passed as an argument in the list.

Extend() Add all items of a list to another list.

Append() Add an element to the end of the list.

Reverse() Reverse the order of elements given in the list.

Clear() Removes all elements from the list.

Index() Returns the index of the first element matched. If the element is not present in the list, it raises ValueError.

pop() Removes and returns an element from a specified index (default is the last one).

Sort() Sorts items in a list.

Insert() Inserts an element at the defined index place.

Remove() Removes the list order.
```

## tuples method

```python
index() Finds in the tuple and returns the index of the specific value where it’s available.

count() Returns the number/frequency of occurrence of a specified value.

all() Returns true if all the elements are true or if the tuple is empty.

enumerate() Returns enumerate objects of the tuple.

sorted() Inputs elements in the tuple and returns a new sorted list.

any() Returns true if an element of the tuple is true. But if the tuple is empty, it returns false.

len() Returns the length or size of the tuple.

max() Returns the maximum element of a given tuple.

min() Returns the minimum element of a given tuple.

sum() Sums up all the numbers in the tuple.

tuple() Converts an iterable to a tuple.
```

## dictionary method

```python
address = {
    "name": "WsCubeTech",
    "location1": "Jodhpur"}

Adding a new key-value pair
address["location2"] = "Jaipur"

print(address["name"])       # Using square brackets
print(address.get("location1"))  # Using get() method

data = {"name": "WsCube", "city": "Jaipur", "course": "Python"}

del data["city"]              # Remove 'city'
print(data.pop("course"))     # Remove and return 'course'
data.popitem()                # Remove last item ('name')
data.clear()                  # Remove everything
print(data)
```

### more dictionary 

```python
dic.clear() Removes all the elements from the dictionary.

dict.copy() Returns a copy of the dictionary.

dict.pop() Removes an element with the specified key.

dict.get() Returns the value of the specified key.

dict.keys() Returns a list of keys of the dictionary.

dict.items() Returns a list with a tuple for each key-value pair.

popItem() Removes the last added key-value pair.

dict.update(dict2) Updates the dictionary with key-value pairs.

dict.get(key, default = “None”) Returns the value specified for the passed key.

dict.setdefault(key,default= “None”) Sets the key to the default value if it is not specified in the dictionary.

dict.values() Returns a list of all the values of the dictionary.

dict.has_key(key) Returns True if the dictionary contains the specified key; else returns False.
```
## sets methods

```python
remove() removes as pecific item

clear() clears the set

pop() removes a random item

Union
a = {1, 2, 3}
b = {3, 4, 5}

print(a.union(b))  
print(a | b)

Output:
{1, 2, 3, 4, 5}


a = {1, 2, 3, 4}
b = {3, 4, 5, 6}

print(a.intersection(b))
print(a & b)

Output:
{3, 4}


a = {1, 2, 3, 4, 5}
b = {3, 4, 6}

print(a.difference(b))
print(a - b)

Output:
{1, 2, 5}


a = {1, 2, 3, 4}
b = {3, 4, 5, 6}

print(a.symmetric_difference(b))
print(a ^ b)

Output:
{1, 2, 5, 6}
```


### other sets methods

```python
add() Adds an element to the set if it doesn’t exist already.

clear() Removes all elements from the set.

remove() Removes an element from the set. If the element is not a member of the set, it raises a KeyError.

discard() Removes the specified element from the set. If the element is not in the set, it doesn’t take any action.

copy() Returns a shallow copy of the set.

difference() Returns the difference between two or more sets as a new set. 

difference_update() Removes elements from this set that are also included in another specified set.

isdisjoint() Returns True if there is a null intersection between two sets.

issubset() Returns True if another set contains this set.

issuperset() Returns True if this set contains another set.

intersection() Returns a new set by intersecting two or more sets.

symmetric_difference() Returns a new set with the symmetric differences of two sets.

symmetric_difference_update() Updates the symmetric difference of this set and another.

union() Returns a new set containing the union of sets.

update() Updates the set with another set.
```

## types conversion 
str()
list()
set()
int()
