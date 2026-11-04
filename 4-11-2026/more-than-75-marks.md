## More Than 75 Marks

Link: [Hackerrank](https://www.hackerrank.com/challenges/more-than-75-marks/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition
Get all students from table STUDENTS. Put a condition to display students who are only scored higher than 75 marks. 

Sort by the forst three Characters and a secondary sort of ID


## Solution

```SQL
SELECT Name
FROM STUDENTS
WHERE Marks > 75
ORDER BY RIGHT(Name, 3) ASC, ID ASC;


```