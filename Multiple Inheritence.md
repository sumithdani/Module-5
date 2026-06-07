# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

##  Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

##  Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

##  Program 
```
class Add:
    def addition(self, a, b):
        print("Addition =", a + b)
class Sub:
    def subtraction(self, a, b):
        print("Subtraction =", a - b)
class Div(Add, Sub):
    def division(self, a, b):
        print("Division =", a / b)
a = int(input())
b = int(input())
obj = Div()
obj.addition(a, b)
obj.subtraction(a, b)
obj.division(a, b)
```
## Output Example
<img width="560" height="361" alt="image" src="https://github.com/user-attachments/assets/02cbfdc4-1bde-461e-9d62-cd06a1d8b507" />

## Result
Thus, the Python program to calculate Addition, Subtraction, and Division using Multiple Inheritance was executed successfully, and the required results were displayed.
