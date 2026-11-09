## Binary Search Tree

Link: [Hackerrank](https://www.hackerrank.com/challenges/binary-search-tree-1/problem?isFullScreen=true)


Difficulty : Medium
DB Engine : MySQL

*********

## Intuition
create a case of all conditions. For not triangle a sum of two sides and less than one side cannot make a triangle. 
Equilateral all sides should be equal
Isosceles only twoi sides should be equal

## Solution

```SQL
SELECT N,
    CASE
        WHEN P IS NULL THEN 'Root'
        WHEN N NOT IN (SELECT P FROM BST WHERE P IS NOT NULL) THEN 'Leaf'
        ELSE 'Inner'
    END AS NodeType
FROM BST
ORDER BY N;
```