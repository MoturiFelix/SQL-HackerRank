## Draw The Triangle 1


Link: [Hackerrank](https://www.hackerrank.com/challenges/draw-the-triangle-1/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition
Print the asterisk pattern according to the current value of n. 
Start with 20. Combine all the initial value with subsequent rows. Decrease the number by 1 each time and stop when it reaches 1. 

## Solution

```SQL
WITH RECURSIVE pattern AS (
    SELECT 20 AS n
    UNION ALL
    SELECT n - 1
    FROM pattern
    WHERE n > 1
)
SELECT REPEAT('* ', n)
FROM pattern;

```

