# Exp.No:22  
## Destructor

---

### AIM  
To write a Python program that creates a class with a constructor to initialize name and age, a method to display them, and a destructor to print a message when the object is destroyed.


### ALGORITHM

1.	Start the program.
2.	Define a class named Person.
3.	Define the __init__ method (constructor) to accept name and age, initialize them, and print "Person Created".
4.	Define a method display() to print the name and age.
5.	Define the __del__ method (destructor) to print a message when the object is destroyed.
6.	Accept name and age as input from the user.
7.	Create an object of the Person class using the input values.
8.	Call the display() method.
9.	Let the destructor automatically trigger when the object goes out of scope.
10.	End the program.



### PROGRAM

```
#Reg.NO:212222060204
#Name:RUPESH J
class Person:
    def __init__(self,name,age):
        print("Person Created")
        self.name = name
        self.age = age
    def printInfo(self):
        print(self.name,self.age)
    def __del__(self):
        print(self.name,"Object Destroyed")

name=input()
age=int(input())
P1=Person(name,age)
#P2=Person("Joe",34)
P1.printInfo()
#P2.printInfo()
del P1
```

### OUTPUT

![image](https://github.com/user-attachments/assets/75a96511-79b4-4eb9-aed5-b1f4bf9a21ab)


### RESULT
Thus, the Python program to demonstrate the use of a constructor, method, and destructor in a class has been implemented and executed successfully.
