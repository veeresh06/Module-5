# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
```
# Class 1
class Calculation1:
    def Summation(self, a, b):
        return a + b


# Class 2
class Calculation2:
    def Subtraction(self, a, b):
        return a - b


# Derived class (Multiple Inheritance)
class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        if b != 0:
            return a / b
        else:
            return "Division by zero not allowed"


# Input
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

# Object creation
obj = Derived()

# Output
print("\n--- Results ---")
print("Addition:", obj.Summation(a, b))
print("Subtraction:", obj.Subtraction(a, b))
print("Division:", obj.Division(a, b))
```
## Output Example
<img width="606" height="438" alt="image" src="https://github.com/user-attachments/assets/ae268800-befd-4261-be0d-9edd4d73622f" />
