# Learned from Caesar Cipher Lab 
https://www.freecodecamp.org/learn/python-v9/workshop-caesar-cipher/step-1

Specifically referencing a part of the lab I was stuck on, the decryption process involved equating the negative of the 'shift' object to be a negative of itself instead of the subtraction of itself. This can be important for similar operations in backend.
```python
# init
shift = 2
# logic
shift -= shift # equates to the subtraction of itself (2 - 2) in this case. It will always be 0.
shift = -shift # equates to the negative of the original value, modifying rather than using an operator. Therefore becoming -2.
```
# Class Init

Classes in Python typically use PascalCase, where the beginning of each word is capitalized throughout the whole class name.
Defining '__init__' in a class, as seen here:
```python
class MusicalInstrument:
  def __init__(self, name, instrument_type):
    self.name = name
    self.instrument_type = instrument_type

instrument_1 = MusicalInstrument('Trumpet', 'brass')
```
This allows for the class to be assigned parameters as soon as an object is defined as a MusicalInstrument.
Why we don't define the parameters in the class line itself is due to the attempt to avoid AttributeErrors.
