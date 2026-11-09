## Revising Aggregations Sum

Link: [Hackerrank](https://www.hackerrank.com/challenges/what-type-of-triangle/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Solution

```SQL
SELECT SUM(POPULATION)
FROM CITY
WHERE DISTRICT = 'California';
```