# Method Memory

find()
- locates first occurance of specified substring within a string
- if no first occurance, returns -1
```python
text = "Hello, World"
print(text.find("World")) # Prints: 7
print(text.find("bruh")) # Prints: -1
```
count()
- locates and determines num of a specific element that appears in a sequence (lists, tuples, strings)
```python
num = [1, 2, 2, 3, 5, 6]
print(num.count(1)) # Prints: 1
print(num.count(2)) # Prints: 2
print(num.count(3)) # Prints: 1
```

isinstance()
- finds the class or type of an object
- very useful for conditional statements involving checks
```python
num = 5
if not isinstance(num, int): # 'if isinstance(num, int):' is also useable here, but I like Boolean algebra :^)
  print('boohoo') # N
else:
  print('yippee') # Y
```

### List Methods

append()
- Adds an item to the end of a list
```python
num = [1, 2, 3]
num.append(4)
print(num) # Prints[1, 2, 3, 4]
```
extend()
- Similar to append(), but adds a list to another at the end of the list
```python
num = [1, 2, 3]
num2 = [4, 5, 6]
num.extend(num2)
print(num) # Prints [1, 2, 3, 4, 5, 6]
```
insert()
- Inserts a specific element to a specific index
```python
num = [1, 2, 3]
num.insert(1, 1.5)
print(num) # Prints [1, 1.5, 2, 3]
```
remove()
- Removes a specific element by its value
```python
num = [1, 2, 3]
num.remove(2)
print(num) # Prints [1, 3]
```
pop()
- Removes a specific element by its index *or* the last indice if not specified
```python
num = [1, 2, 3]
num.pop(0)
print(num) # Prints [2, 3]
num.pop()
print(num) # Prints [2]
```
clear()
- Clears the list
```python
num = [1, 2, 3]
num.clear()
print(num) # Prints [ ]
```
sort() and sorted()
- sort() functions as a modification for a list, and directly modifies the variable by sorting a list either numerically or alphabetically (case-sensitive)
- sorted() creates a new list entirely, defining a new variable by being the sorted() of x, x being an already defined list.
```python
num_unsorted = [2, 3, 1.5, 1]
num_sorted = sorted(num_unsorted)
print(num_sorted) # Prints [1, 1.5, 2, 3]
print(num_unsorted) # Still prints [2, 3, 1.5, 1], but sort() modifies
sort(num_unsorted)
print(num_unsorted) # Now prints [1, 1.5, 2, 3]
```
reverse()
- Reverses a list, ***does not sort***
```python
num = [1, 3, 2]
num.reverse()
print(num) # Prints [2, 3, 1]
```
index()
- Finds a specific element by its value in a string and returns its index
```python
num = [1, 2, 3]
num.index(2) # returns 1
```
