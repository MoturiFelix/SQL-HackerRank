## Revising Aggregations The Count Function


Link: [Hackerrank](https://www.hackerrank.com/challenges/revising-aggregations-the-count-function/problem?isFullScreen=true)


DB Engine : MySQL

*********

## Intuition

We will have to use the Count function for this.


## Solution

```SQL
SELECT COUNT(NAME)
FROM CITY
WHERE POPULATION > 100000;
```