# Exp.No:24  
## Multi-level Inheritance

---

### AIM  
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

---

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.

2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `person_id` to `self.person_id`.

3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `person_id`.

4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.person_id`.

5. Prompt the user to enter `name` (string), `age` (integer), and `person_id` (integer).

6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `person_id` to the constructor.

7. Call the `show_details` method on the `person` object and print the result.

8. Terminate the program.

---

### PROGRAM
```
class Person:
    def __init__(self):
        self.name = ""
    def get_name(self):
        self.name = input()
class Age(Person):
    def __init__(self):
        super().__init__()
        self.age = 0
    def get_age(self):
        self.age = int(input())
class Salary(Age):
    def __init__(self):
        super().__init__()
        self.salary = 0
    def get_salary(self):
        self.salary = float(input())
    def display(self):
        print(self.name, self.age, int(self.salary))
emp = Salary()
emp.get_name()
emp.get_age()
emp.get_salary()
emp.display()
```
### OUTPUT

<img width="827" height="226" alt="image" src="https://github.com/user-attachments/assets/2e5d9357-05ec-4d10-ba23-644924e42d4e" />

### RESULT

Thus, the python code is written and executed successfully.
