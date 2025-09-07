# Exp.No:22  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM
```
class Employee:
	def __init__(self):
		print('Employee created.')
	def __del__(self):
		print('Destructor called, Employee deleted.')
obj = Employee()
del obj
```
### OUTPUT

<img width="835" height="267" alt="image" src="https://github.com/user-attachments/assets/03fd8dae-8222-48ed-bd29-7e0506c9ef37" />

### RESULT
Thus, the python code is written and executed successfully.
