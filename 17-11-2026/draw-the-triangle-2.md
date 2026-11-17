## Draw the Triangle 2


Link: [Hackerrank](https://www.hackerrank.com/challenges/draw-the-triangle-2/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition

Print the asterisk pattern according to the current value of n. 
Start with 1. Combine all the initial value with subsequent rows. Increase the number by 1 each time and stop when it reaches 20. 


## Solution

```SQL
WITH RECURSIVE pattern AS (
    SELECT 1 AS n
    UNION ALL
    SELECT n + 1
    FROM pattern
    WHERE n < 20
)
SELECT REPEAT('* ', n)
FROM pattern;
```

