Payroll System
This Java program implements a simple payroll management system that allows the user to manage full-time and part-time employees. The system provides functionalities to add employees, remove employees, and display employee details, including their calculated salaries.

Table of Contents
Features
Class Structure
Employee
FullTimeEmployee
PartTimeEmployee
PayrollSystem
Main Class
Getting Started
Usage
Sample Output
Features
Add Full-Time and Part-Time Employees: Users can add new employees to the payroll system.
Remove Employees: Users can remove employees by their unique ID.
Display Employees: Users can view a list of all employees and their respective salaries.
Calculate Salaries: Automatically calculates salaries for both full-time and part-time employees based on their input details.
Class Structure
1. Employee (Abstract Class)
The Employee class is an abstract class that serves as the base class for all employee types. It contains:

Private fields name and id for storing employee details.
Constructor for initializing name and id.
Getter methods for retrieving name and id.
An abstract method calculateSalary() to be implemented by subclasses.
A toString() method for displaying employee information.
2. FullTimeEmployee (Subclass of Employee)
The FullTimeEmployee class extends the Employee class. It represents a full-time employee and contains:

A private field monthlySalary to store the monthly salary of the employee.
A constructor to initialize the employee details and monthlySalary.
An implementation of the calculateSalary() method that returns the monthlySalary.
3. PartTimeEmployee (Subclass of Employee)
The PartTimeEmployee class extends the Employee class. It represents a part-time employee and contains:

Private fields hoursWorked and hourlyRate to store the number of hours worked and the hourly rate.
A constructor to initialize the employee details, hoursWorked, and hourlyRate.
An implementation of the calculateSalary() method that calculates and returns the salary as hoursWorked * hourlyRate.
4. PayrollSystem
The PayrollSystem class manages the list of employees and contains:

A private employeeList field to store a list of employees.
addEmployee(Employee employee) method to add an employee to the list.
removeEmployee(int id) method to remove an employee from the list by their ID.
displayEmployees() method to display the list of employees along with their details.
5. Main Class
The Main class contains the main() method, which provides a command-line interface (CLI) for interacting with the payroll system. It allows users to:

Add full-time and part-time employees.
Remove employees by their ID.
Display the list of all employees.
Exit the application.
The Main class uses a Scanner to read user input and performs operations based on user choices.

Getting Started
Prerequisites
Java Development Kit (JDK) installed on your system.
Running the Program
Copy the source code into a file named Main.java.
Open a terminal and navigate to the directory containing Main.java.
Compile the code using the following command:
bash
Copy code
javac Main.java
Run the compiled program using the command:
bash
Copy code
java Main
Usage
Add Full-Time Employee: Select option 1 from the menu, enter the employee's name, ID, and monthly salary.
Add Part-Time Employee: Select option 2 from the menu, enter the employee's name, ID, hours worked, and hourly rate.
Remove Employee: Select option 3 and enter the employee ID to remove them from the system.
Display Employees: Select option 4 to display the list of all employees with their details.
Exit: Select option 5 to exit the program.
Sample Output
mathematica
Copy code
Payroll System Menu:
1. Add Full-Time Employee
2. Add Part-Time Employee
3. Remove Employee
4. Display Employees
5. Exit
Enter your choice: 1

Enter Full-Time Employee Name: John Doe
Enter Employee ID: 101
Enter Monthly Salary: 5000
Full-Time Employee Added Successfully!

Payroll System Menu:
1. Add Full-Time Employee
2. Add Part-Time Employee
3. Remove Employee
4. Display Employees
5. Exit
Enter your choice: 4

Employee Details:
Employee [name=John Doe, id=101, salary=5000.0]
Conclusion
This payroll system provides a simple and effective way to manage employees and their salaries. The design utilizes Object-Oriented Programming (OOP) concepts such as inheritance and abstraction, providing a modular and extendable structure.

Feel free to extend the functionality as needed to suit more complex payroll management requirements!
