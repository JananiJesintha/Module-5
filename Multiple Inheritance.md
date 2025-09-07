# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible.

---

### ALGORITHM

1. Define the `Student` class.
2. Inside the `Student` class, define the `__init__` method (constructor). The `__init__` method accepts two parameters: `name` and `student_id`.
    - Inside the `__init__` method: Assign the value of `name` to `self.name` and `student_id` to `self.student_id`.
3. Define the `get_student_info` method inside the `Student` class:
    - This method should return a string formatted with `self.name` and `self.student_id`.
4. Define the `Attendance` class, which inherits from the `Student` class.
5. Inside the `Attendance` class, define the `__init__` method (constructor).
    - The `__init__` method accepts three parameters: `name`, `student_id`, and `attendance`.
    - Inside the `__init__` method: Call the parent class constructor `super().__init__(name, student_id)` to initialize `name` and `student_id`. Assign the value of `attendance` to `self.attendance`.
6. Define the `check_eligibility` method inside the `Attendance` class:
    - If `self.attendance` is greater than 80, return a formatted string indicating the student is eligible for the module exam.
    - Otherwise, return a formatted string indicating the student is not eligible for the module exam.
7. Prompt the user to enter the `name` (as a string), `student_id` (as an integer), and `attendance` (as an integer).
8. Create an instance `student` of the `Attendance` class, passing the entered `name`, `student_id`, and `attendance` to the constructor.
9. Call the `check_eligibility` method on the `student` object and print the result.
10. Terminate the program.

---

### PROGRAM
```
class Student:
    def __init__(self, name, student_id, attendance):
        self.name = name
        self.student_id = student_id
        self.attendance = attendance
class Eligibility:
    def check_eligibility(self, attendance):
        if attendance > 80:
            return "Eligible for Module Exam"
        else:
            return "Not Eligible for Module Exam"
class StudentEligibility(Student, Eligibility):
    def display(self):
        eligibility = self.check_eligibility(self.attendance)
        print(self.name)
        print(self.student_id)
        print(eligibility)
name = input()
student_id = int(input())
attendance = int(input())
student = StudentEligibility(name, student_id, attendance)
student.display()
```
### OUTPUT

<img width="823" height="307" alt="image" src="https://github.com/user-attachments/assets/b7d9bc8d-6d70-41a7-8a75-4c87db7ff7d8" />

### RESULT

Thus, the python code is written and executed successfully.
