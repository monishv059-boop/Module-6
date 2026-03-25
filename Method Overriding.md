# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
~~~
class Fish:
    def type(self):
        print("fish")

class Shark(Fish):
    def type(self):
        print("shark")

obj_goldfish = Fish()
obj_hammerhead = Shark()

print("Output:")
for obj in [obj_goldfish, obj_hammerhead]:
    obj.type()

Result = ["fish", "shark"]



~~~

## OUTPUT
<img width="1560" height="989" alt="530372729-7a6c043e-6ea4-42e9-a4f1-32679258b1b7" src="https://github.com/user-attachments/assets/856e5c21-2f25-4df1-943e-c038602e095c" />

## RESULT
The program successfully demonstrates class inheritance by creating a parent class Fish with a method type, and a child class Shark that overrides the type method.
