# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program using hierarchical inheritance where a base class Details is inherited by two derived classes Employee and Doctor to store and display their respective details.

---

### ALGORITHM
1.	Start the program.
2.	Define a base class Details with a constructor to initialize id, name, and gender.
3.	Define a class Employee that inherits from Details.
4.	In the Employee class, define a constructor that calls the base class constructor and initializes company and department.
5.	Define a display() method in the Employee class to print employee details.
6.	Define another class Doctor that also inherits from Details.
7.	In the Doctor class, define a constructor that calls the base class constructor and initializes hospital and department.
8.	Define a display() method in the Doctor class to print doctor details.
9.	Accept user inputs for both employee and doctor details.
10.	Create instances of Employee and Doctor using the input values.
11.	Call the display() method for both instances to show their details.
12.	End the program.


### PROGRAM
```
#Reg.NO:212222060204
#Name:RUPESH J
class Details:
    def __init__(self, emp_id, name, gender):
        self.emp_id = emp_id
        self.name = name
        self.gender = gender

class Employee(Details):
    def __init__(self, emp_id, name, gender, company, department):
        super().__init__(emp_id, name, gender)  
        self.company = company
        self.department = department

    def display_employee(self):
        return (f"Employee Object\n"
                f"Id:  {self.emp_id}\n"
                f"Name:  {self.name}\n"
                f"Gender:  {self.gender}\n"
                f"Company:  {self.company}\n"
                f"Department:  {self.department}")

class Doctor(Details):
    def __init__(self, emp_id, name, gender, hospital, department):
        super().__init__(emp_id, name, gender)
        self.hospital = hospital
        self.department = department

    def display_doctor(self):
        return (f"Doctor Object\n"
                f"Id:  {self.emp_id}\n"
                f"Name:  {self.name}\n"
                f"Gender:  {self.gender}\n"
                f"Hospital:  {self.hospital}\n"
                f"Department:  {self.department}")

if __name__ == "__main__":
    # Input for Employee
    emp_id = int(input())
    emp_name = input()
    emp_gender = input()
    emp_company = input()
    emp_department = input()

    employee = Employee(emp_id, emp_name, emp_gender, emp_company, emp_department)

    doc_id = int(input())
    doc_name = input()
    doc_gender = input()
    doc_hospital = input()
    doc_department = input()

    doctor = Doctor(doc_id, doc_name, doc_gender, doc_hospital, doc_department)

    print(employee.display_employee())
    print()
    print(doctor.display_doctor())


```

### OUTPUT  

![image](https://github.com/user-attachments/assets/58d8d741-ca3a-4a18-9aea-34d208312683)


### RESULT
Thus, the Python program to demonstrate hierarchical inheritance using Details, Employee, and Doctor classes has been implemented and executed successfully.
