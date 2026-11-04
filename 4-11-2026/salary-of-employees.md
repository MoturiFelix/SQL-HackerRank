## Salary of Employees

Link: [Hackerrank](https://www.hackerrank.com/challenges/salary-of-employees/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition
Display a list of employees who earn a salary greater than $2000 from the employee table. The employees displayed should have worked for less than 10 months. 


## Solution

```SQL
SELECT NAME FROM EMPLOYEE
WHERE SALARY > 2000 AND MONTHS < 10;

```