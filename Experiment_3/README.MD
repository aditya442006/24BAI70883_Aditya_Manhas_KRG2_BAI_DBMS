1. Aim 
To understand the basic structure of a PL/SQL program by creating and executing a simple PL/SQL block that includes declaration and execution sections, and to display output using built-in procedures.

2. Objective of the Session
•	To understand the basic structure of an Oracle PL/SQL block
•	To learn variable declaration and initialization in PL/SQL
•	To implement procedural logic using the BEGIN–END execution block
•	To display output using built-in procedures such as DBMS_OUTPUT.PUT_LINE
•	To strengthen foundational PL/SQL skills required for database programming, backend development, and technical interviews
.
3. Theory
1. A PL/SQL block consists of three main sections:
Declaration Section (DECLARE)
o	Variables, constants, cursors are declared here.
Execution Section (BEGIN … END)
o	Contains executable statements.
Exception Section (EXCEPTION) (optional)
Think of it like a human:
•	DECLARE → Memory
•	BEGIN → Action
•	END → Closure
4. Problem Statement
Design and implement a simple PL/SQL program that demonstrates the basic structure of a PL/SQL block.
The program should:
1.	Declare variables for employee details
2.	Assign values to those variables
3.	Display the values using output statements

5. Procedure of the Practical
1.	Open pgAdmin / SQL environment (conceptual PL/SQL execution).
2.	Enable server output:
3.	SET SERVER OUTPUT ON;
4.	Write a PL/SQL block with:
•	Employee ID
•	Employee Name
•	Employee Salary
5.	Assign values inside the execution section.
6.	Display output using DBMS_OUTPUT.PUT_LINE.
7.	Execute the block and observe the output.


5. I/O Analysis (Input / Output Analysis)
Input: 
Variable 	Value
Emp_id	
	101

Emp_name	
	Aditya 

Emp_salary	
	45000


Output: 
Employee ID     : 101
Employee Name   : Aditya Manhas
Employee Salary : 45000
SQL Implementation (PgAdmin / PostgreSQL)
DECLARE
    emp_id      NUMBER := 101;
    emp_name    VARCHAR2(50) := 'Aditya ';
    emp_salary  NUMBER := 45000;
BEGIN
    DBMS_OUTPUT.PUT_LINE('Employee Details');
    DBMS_OUTPUT.PUT_LINE('----------------');
    DBMS_OUTPUT.PUT_LINE('Employee ID    : ' || emp_id);
    DBMS_OUTPUT.PUT_LINE('Employee Name  : ' || emp_name);
    DBMS_OUTPUT.PUT_LINE('Employee Salary: ' || emp_salary);
END;
7. Learning Outcomes
•	Understand the basic structure of a PL/SQL block
•	Declare and initialize variables in PL/SQL
•	Use the BEGIN–END execution block
•	Display output using DBMS_OUTPUT.PUT_LINE
•	Develop confidence in writing simple procedural database programs

7.  Screenshots
•	 C:\Users\ASUS\OneDrive\Documents\Experiment_3\screenshot.jpeg

