# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
To write a Python code to create a class for a person with a parameterized constructor, which will take the `name` and `userid` of the person as parameters and print the `userid` of the person.

---

### ALGORITHM

1. Begin the program.  
2. Define a `person` class.  
3. The `person` class should have a parameterized `__init__` method that accepts two parameters: `name` and `userid`.  
4. Inside the `__init__` method, assign the `name` to `self.name` and the `userid` to `self.userid`.  
5. Print the `self.userid`.  
6. Prompt the user to enter their `name` (string) and `userid`.  
7. Create an instance `s1` of the `person` class by passing the entered `name` and `userid` to the constructor.  
8. Terminate the program.

---

### PROGRAM
```
class addition:
    def __init__(self,a,b):
        self.a = a
        self.b = b
    def summation(self):
        return self.a + self.b
a=int(input())
b=int(input())
result = addition(a,b)
print(f"First number = {a}")
print(f"Second number = {b}")
print("Addition of two numbers =",result.summation())
```
### OUTPUT

<img width="842" height="373" alt="image" src="https://github.com/user-attachments/assets/b00fa424-1f79-4be8-8fc7-8aad98102a1c" />

### RESULT

Thus, the python code is written and executed successfully.
