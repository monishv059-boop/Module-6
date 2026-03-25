# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
~~~
from abc import ABC, abstractmethod
import math

class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass

class Rectangle(Shape):
    def __init__(self, length=5, breadth=10):
        self.length = length
        self.breadth = breadth
    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
    def __init__(self, radius=7):
        self.radius = radius
    def calculate_area(self):
        return math.pi * self.radius**2

rect = Rectangle()
circ = Circle()

print("Output:")
print("Rectangle area:", rect.calculate_area())
print("Circle area:", circ.calculate_area())

Result = (rect.calculate_area(), circ.calculate_area())
~~~

## Output
<img width="1617" height="987" alt="530372359-50e25293-d410-48cd-baed-176221a41cbb" src="https://github.com/user-attachments/assets/80bd72e9-f621-4172-b572-d5fa8bb44a67" />

## Result
The program successfully creates an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle.
