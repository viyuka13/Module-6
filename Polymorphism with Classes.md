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
## Output
![image](https://github.com/user-attachments/assets/e8f45ddb-5a6d-480a-9ef8-f5a6a7a2835d)

## Result
This program shows polymorphism. It has two classes, Beans and Mango, with the same methods that print different messages. The function func() calls these methods for any object passed to it. When Beans and Mango objects are used, the program prints their specific messages.
