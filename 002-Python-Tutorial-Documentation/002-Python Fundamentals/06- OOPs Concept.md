### OOPs Concepts in Python ###

---

Python supports Object-Oriented Programming (OOP), which allows modeling real-world entities using objects, classes, and various other concepts. Below are the key OOP concepts:

---

**Classes and Objects:**  
Classes are blueprints for objects, defining their properties and behavior. Objects are instances of classes.

**Example (class and object):**
```python
class Vehicle:
    def drive(self):
        print("Driving...")

# Create an object
my_vehicle = Vehicle()
my_vehicle.drive()
```

---

**Inheritance:**  
Inheritance allows a class to use properties and behavior of another class. This promotes reusability and extensibility.

**Example (inheritance):**
```python
class Vehicle:
    def drive(self):
        print("Driving...")

class Car(Vehicle):  # Car inherits from Vehicle
    def accelerate(self):
        print("Accelerating...")

my_car = Car()
my_car.drive()        # Inherited method
my_car.accelerate()   # Subclass-specific method
```

---

**Polymorphism:**  
Polymorphism allows methods to do different things based on the object they are acting upon. It is achieved through method overriding and method overloading (to a limited extent in Python).  

**Example (method overriding):**
```python
class Vehicle:
    def drive(self):
        print("Driving...")

class Car(Vehicle):
    def drive(self):  # Method overriding
        print("Driving a car...")

my_vehicle = Vehicle()
my_vehicle.drive()

my_car = Car()
my_car.drive()  # Polymorphism
```

---

**Encapsulation:**  
Encapsulation involves wrapping data (attributes) and code (methods) together and controlling access to them.

**Example (encapsulation):**
```python
class BankAccount:
    def __init__(self, balance):
        self.__balance = balance  # Private attribute

    def deposit(self, amount):
        self.__balance += amount

    def get_balance(self):
        return self.__balance

account = BankAccount(1000)
account.deposit(500)
print(account.get_balance())  # Accessing through a method
```

---

**Abstraction:**  
Abstraction focuses on representing the essential features without exposing unnecessary details. This is achieved using abstract base classes (ABC) in Python.

**Example (abstraction):**
```python
from abc import ABC, abstractmethod

class Vehicle(ABC):
    @abstractmethod
    def drive(self):
        pass

class Car(Vehicle):
    def drive(self):
        print("Driving a car...")

my_car = Car()
my_car.drive()
```

---

Python's OOP features allow for creating well-structured, modular, and reusable code for real-world applications.