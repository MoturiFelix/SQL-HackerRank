## What type of Triangle

Link: [Hackerrank](https://www.hackerrank.com/challenges/what-type-of-triangle/problem?isFullScreen=true)


Difficulty : Medium
DB Engine : MySQL

*********

## Intuition
create a case of all conditions. For not triangle a sum of two sides and less than one side cannot make a triangle. 
Equilateral all sides should be equal
Isosceles only twoi sides should be equal


## Solution

```SQL
SELECT
    CASE
        WHEN A + B <= C OR A + C <= B OR B + C <= A
            THEN 'Not A Triangle'
        WHEN A = B AND B = C
            THEN 'Equilateral'
        WHEN A = B OR B = C OR A = C
            THEN 'Isosceles'
        ELSE 'Scalene'
    END AS Triangle_Type
FROM TRIANGLES;

```