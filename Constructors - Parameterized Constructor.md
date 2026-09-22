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

# Reg.No: 212223060129
# Name: KOWSALYA V


class employees:
    def __init__(self,a,b):
        self.a=a
        self.b=b
    def dis(self):
        print("Hello my id is :",a)
        print("My name is :",b)
a=int(input())
b=input()
obj=employees(a,b)
obj.dis()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/6146f96d-383e-48d6-95e8-23fb2e57fac6)


### RESULT
Thus,a Python code to create a class for a person with a parameterized constructor are verified.
