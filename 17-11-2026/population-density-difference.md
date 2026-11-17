## Population Density Difference


Link: [Hackerrank](https://www.hackerrank.com/challenges/population-density-difference/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition

Select the Maximum population and Minimum and get the difference


## Solution

```SQL
SELECT COUNT(NAME)
FROM CITY
WHERE POPULATION > 100000;
```

