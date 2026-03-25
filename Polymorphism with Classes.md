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
~~~
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

beans = Beans()
mango = Mango()

print("Output:")
func(beans)
func(mango)

Result = [("Vegetable", "Green"), ("Fruit", "Yellow")]

~~~

## Output
<img width="1544" height="983" alt="530373160-ad7f0ac7-e99f-4949-be89-52323dae799a" src="https://github.com/user-attachments/assets/5f8ad3b1-3132-4ad2-878e-2ae217e3d8bc" />

## Result
The program successfully creates two specific classes — Beans and Mango. Then, create a generic function that can accept any object and determine its type (Fruit or Vegetable) and color, using polymorphism.
