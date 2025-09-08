# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program that performs addition, multiplication, and division using multiple inheritance.


---

### ALGORITHM
1.	Start the program.
2.	Define class Add with method add() to perform addition.
3.	Define class Mul with method mul() to perform multiplication.
4.	Define class Div that inherits from Add and Mul, and define method div() for division.
5.	Read two integer inputs from the user.
6.	Create an object of class Div.
7.	Call the add(), mul(), and div() methods and display the results.
8.	End the program.

### PROGRAM

```
#Reg.NO:212222060204
#Name:RUPESH J
class Addition:
    def add(self, a, b):
        return a + b

class Multiplication:
    def multiply(self, a, b):
        return a * b

class Division:
    def divide(self, a, b):
        if b != 0:
            return a / b
        else:
            return "Division by zero is not allowed."

class Calculator(Addition, Multiplication, Division):
    def calculate(self, a, b):
        addition = self.add(a, b)
        multiplication = self.multiply(a, b)
        division = self.divide(a, b)
        return addition, multiplication, division

if __name__ == "__main__":
    num1 = int(input())
    num2 = int(input())
    calc = Calculator()
    add_result, mul_result, div_result = calc.calculate(num1, num2)
    print(f"{add_result}")
    print(f"{mul_result}")
    print(f"{div_result}")

```

### OUTPUT

![LAB5 MULTIPLE](https://github.com/user-attachments/assets/47198c4f-1820-41cd-be91-997cad57fec3)


### RESULT
Thus, the Python program to perform addition, multiplication, and division using multiple inheritance has been implemented and executed successfully.



