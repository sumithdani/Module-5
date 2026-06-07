# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

##  Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

##  Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

##  Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
```
class Person:
    def get_person(self):
        self.name = input("Enter Name: ")
        self.age = int(input("Enter Age: "))

class Employee(Person):
    def get_employee(self):
        self.empid = input("Enter Employee ID: ")

    def display_employee(self):
        print("\nEmployee Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.empid)

class Patient(Person):
    def get_patient(self):
        self.pid = input("Enter Patient ID: ")

    def display_patient(self):
        print("\nPatient Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.pid)

e = Employee()
e.get_person()
e.get_employee()
e.display_employee()

p = Patient()
p.get_person()
p.get_patient()
p.display_patient()
```
## Sample Output
<img width="642" height="697" alt="image" src="https://github.com/user-attachments/assets/194b1f21-b79a-4d20-b326-6dc9969c48b4" />

## Result
Thus, the Python program using Hierarchical Inheritance to input and display Employee and Patient details was executed successfully, and the required details were displayed.
