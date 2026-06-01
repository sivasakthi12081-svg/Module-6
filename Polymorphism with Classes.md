# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
```
class Beans:
    def type(self):
        print("Vegetable")
    def color(self):
        print("Green")
        
class Mango:
    def type(self):
        print("Fruit")
    def color(self):
        print("Yellow")
        
def func(obj):
    obj.type()
    obj.color()
b = Beans()
m = Mango()
func(b)
func(m)
```

## Output
<img width="1910" height="974" alt="Screenshot 2026-06-01 235919" src="https://github.com/user-attachments/assets/fc24be64-0253-470d-bb7a-024b4deb6a2d" />

## Result
The same function func(obj) works with different objects (Beans, Mango).
This demonstrates polymorphism — different objects respond to the same method calls in their own way.
