## The Pads

Link: [Hackerrank](https://www.hackerrank.com/challenges/the-pads/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition
Extract the first letter of each occupation, combine it with the person's name, and sort the names alphabetically.

Group people by occupation, count each group, convert occupation names to lowercase, format the results as sentences, and sort by count in ascending order, then alphabetically when counts are equal.




## Solution

```SQL
SELECT CONCAT(Name, '(', LEFT(Occupation, 1), ')')
FROM OCCUPATIONS
ORDER BY Name ASC;


SELECT CONCAT(
    'There are a total of ',
    COUNT(*),
    ' ',
    LOWER(Occupation),
    's.'
)
FROM OCCUPATIONS
GROUP BY Occupation
ORDER BY COUNT(*) ASC, Occupation ASC;

```
