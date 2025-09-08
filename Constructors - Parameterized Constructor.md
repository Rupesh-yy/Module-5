# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
To write a Python program that defines a class with a parameterized constructor accepting a name and displaying a greeting message using a method.

---

### ALGORITHM

1.	Begin the program.
2.	Define a class Name.
3.	Define the constructor __init__ to accept a single parameter name.
4.	Assign the input value to the instance variable self.name.
5.	Define a method display() to print a greeting with the name.
6.	Take the user input for name.
7.	Create an object of the Name class using the input.
8.	Call the display() method.
9.	Terminate the program.


### PROGRAM

```
#Reg.NO:212222060204
#Name:RUPESH J
class Name:
    def __init__(self,name):
        self.name = name
        
    def display(self):
        print("Hello "+ self.name)

name = input()
s = Name(name)
print("This is non parametrized constructor")
s.display()
```

### OUTPUT

![image](https://github.com/user-attachments/assets/308888d4-141d-4c2b-b929-7b381b20a1b8)


### RESULT
Thus, the Python program to create a class with a parameterized constructor that accepts a name and displays a greeting using a class method has been implemented and executed successfully.
