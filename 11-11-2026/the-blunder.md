## the-blunder

## What type of Triangle

Link: [Hackerrank](https://www.hackerrank.com/challenges/the-blunder/problem?isFullScreen=true)


DB Engine : MySQL

*********

## Intuition
get the avarage salary using AVG(Salary). Also, remove all Zeros to get the wrong calculatrion she did. Get the difference and round it off to the nextr integer. 


## Solution

```SQL
SELECT CEIL(
    AVG(Salary) - AVG(REPLACE(Salary, '0', ''))
)
FROM EMPLOYEES;

```