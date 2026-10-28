 ## Revising The Select Query 2

Link: [Hackerrank](https://www.hackerrank.com/challenges/the-pads/problem?isFullScreen=true)


Difficulty : Medium
DB Engine : MySQL

*********

## Intuition
The first question I need every person's name, I need the first letter of their occupation, and I need to combine them into one output. That's why we use LEFT() to get the first letter and || to join the text together. Since the question also asks for alphabetical order, we use ORDER BY Name.

The Second Question I need to group people with the same occupation, count how many are in each group, format the result as a sentence, and sort the counts. That's why we use GROUP BY Occupation to create groups and COUNT(*) to count people in each group. We use LOWER() to make occupation names lowercase and || to construct the sentence. Finally, ORDER BY COUNT(*), Occupation sorts from the smallest count to the largest, then alphabetically when counts are equal.

## Solution

```SQL
SELECT Name || '(' || LEFT(Occupation, 1) || ')'
FROM OCCUPATIONS
ORDER BY Name;
SELECT 'There are a total of ' || COUNT(*) || ' ' || LOWER(Occupation) || 's.'
FROM OCCUPATIONS
GROUP BY Occupation
ORDER BY COUNT(*), Occupation;
```