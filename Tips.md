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
