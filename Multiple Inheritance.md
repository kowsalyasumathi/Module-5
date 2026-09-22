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
# Reg.No: 212223060129
# Name: KOWSALYA V

class Student:
    def __init__(self, name, student_id):
        self.name = name
        self.student_id = student_id

    def get_student_info(self):
        return f"Name: {self.name}, ID: {self.student_id}"

class Attendance(Student):
    def __init__(self, name, student_id, attendance):
        super().__init__(name, student_id)
        self.attendance = attendance

    def check_eligibility(self):
        if self.attendance > 80:
            return f"{self.get_student_info()} is Eligible for Module Exam."
        else:
            return f"{self.get_student_info()} is Not Eligible for Module Exam."

# Taking inputs
name = input()
student_id = int(input())
attendance = int(input())

# Creating object
student = Attendance(name, student_id, attendance)

# Checking eligibility
print(student.check_eligibility())

```

### OUTPUT
![image](https://github.com/user-attachments/assets/c13a2a45-56db-4ede-b4c0-9ca07c96a46f)



### RESULT
Thus a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible has been mplemented successfully.
