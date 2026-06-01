# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length      
        self.__breadth = breadth   
        self.display()
        
    def display(self):
        print("Length =", self.__length)
        print("Breadth =", self.__breadth)
r = Rectangle(10, 5)
```
## Output
<img width="1911" height="764" alt="Screenshot 2026-06-01 235211" src="https://github.com/user-attachments/assets/86b1243c-142b-4250-a8d3-830de8945795" />

## Result
The variables __length and __breadth are private members (encapsulation).
They can be accessed only within the class, not directly from outside.
