## Average Population

Link: [Hackerrank](https://www.hackerrank.com/challenges/average-population-of-each-continent/problem?isFullScreen=true)


DB Engine : MySQL

*********

## Intuition

Get the average population from the city table. Round of to the nearest integer


## Solution

```SQL
SELECT FLOOR(AVG(POPULATION))
FROM CITY
```