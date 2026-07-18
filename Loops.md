# Loops

### for Loop
- for loops follow a sequence of defining by something defined, followed by the body that acts as the instructions in this definiton
```python
# As mentioned, foods_fruits will be our "defined"
foods_fruits = ['Apple', 'Banana', 'Raspberry', 'Orange']
# following the defined, we will define what we want out of the list
for fruits in foods_fruits:
  print(fruits)
# This will return the following:
# Apple
# Banana
# Raspberry
# Orange
# To explain, the fruits defined in the for loop is the elements in the list, using the predefined list as its source.
# This can also be done using something not predefined in a previous line of code, like a string
for char in 'fruit':
  print(char)
# This will return the following:
# f
# r
# u
# i
# t
# You can also place a for loop inside of another for loop, this is a called a nested for loop
good_or_bad = ['Good', 'Bad']
foods = ['Apple', 'Orange', 'Banana']
for describer in good_or_bad:
  for food in foods:
    print(describer, food)
# This will return the following:
# Good Apple
# Good Orange
# Good Banana
# Bad Apple
# Bad Orange
# Bad Banana
```
### while Loop
- while loops follow a more straightforward conditional statement, while a value or condition exists or does not exist (= or !=), follow the logic of the body
```python
secret = 2
input = 0

while input != secret:
  input = int(input('Guess the digit: '))
  if input != secret:
    print('Wrong. Try again.')
print('You got it. :)')
```
### enumerate()
- enumerate finds and gives the indice of the given value
- while not unique loops, it allows for iterative logic and tracking
```python
for price in enumerate(products.values()):
  print(price)
# This will return the following: (with p being price and n being its indice)
# (0, p0)
# (1, p1)
# (2, p2)
```
