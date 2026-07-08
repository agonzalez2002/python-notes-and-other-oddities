# Method Memory

find()
- locates first occurance of specified substring within a string
- if no first occurance, returns -1
- ex:

```python
text = "Hello, World"
print(text.find("World")) # Prints: 7
print(text.find("bruh")) # Prints: -1
```

count()
- locates and determines num of a specific element that appears in a sequence (lists, tuples, strings)
- ex:

```python
num = [1, 2, 2, 3, 5, 6]
print(num.count(1)) # Prints: 1
print(num.count(2)) # Prints: 2
print(num.count(3)) # Prints: 1
```
