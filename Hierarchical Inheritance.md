# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
```
class Value:
    def __init__(self,mul1,mul2):
        self.mul1 = mul1
        self.mul2 = mul2
    def display(self):
        print(" multiplication value1 : ",self.mul1)
        print(" multiplication value2 : ",self.mul2)
class Result(Value):
    def final(self):
        self.display()
        print(" Multiplied value :",self.mul1 * self.mul2)
mul1 = int(input())  
mul2 = int(input())  
obj = Result(mul1,mul2)
obj.final()
```
### OUTPUT  

<img width="827" height="220" alt="image" src="https://github.com/user-attachments/assets/9dc4fe6a-4ff7-465e-8c75-d47877aeb0d7" />

### RESULT

Thus, the python code is written and executed successfully.
