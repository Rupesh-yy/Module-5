# Exp.No:24  
## Multi-level Inheritance

---

### AIM  
To write a Python program using multilevel inheritance to get the name, roll number, and marks of a student and display the total marks.

### ALGORITHM

1.	Start the program.
2.	Define the base class Student with a constructor to initialize name and rollno.
3.	Define the derived class Marks that inherits from Student.
   o	Initialize m1, m2, and m3 as marks of 3 subjects.
4.	Define the next derived class Result that inherits from Marks.
   o	Define a method display() to compute the total and display the student details.
5.	Read inputs from the user for name, rollno, and marks in 3 subjects.
6.	Create an object of the Result class and call the display() method.
7.	End the program.



### PROGRAM

```
#Reg.NO:212222060204
#Name:RUPESH J
class Student:
    def __init__(self, name, roll_no):
        self.name = name
        self.roll_no = roll_no

class Marks(Student):
    def __init__(self, name, roll_no, marks1, marks2, marks3):
        super().__init__(name, roll_no)  
        self.marks1 = marks1
        self.marks2 = marks2
        self.marks3 = marks3

class TotalMarks(Marks):
    def __init__(self, name, roll_no, marks1, marks2, marks3):
        super().__init__(name, roll_no, marks1, marks2, marks3)  

    def calculate_total(self):
        return self.marks1 + self.marks2 + self.marks3
    def display_details(self):
        total = self.calculate_total()
        return f"Name:  {self.name} Rollno:  {self.roll_no} Total Marks out of 300:  {total}"


if __name__ == "__main__":
    name = input()
    roll_no = int(input())
    marks1 = int(input())
    marks2 = int(input())
    marks3 = int(input())

    student = TotalMarks(name, roll_no, marks1, marks2, marks3)
    print(student.display_details())


```

### OUTPUT

![LAB5 MULTILEVEL](https://github.com/user-attachments/assets/e04928eb-dd05-4ae7-899b-ebf23c6230a6)


### RESULT
Thus, the Python program to compute and display the total marks of a student using multilevel inheritance has been implemented and executed successfully.








