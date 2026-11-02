## Weather Observation Station 6

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-6/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition

Pick City from Table Station. Where there is no repeated city. 
Only include cities that start with a vowel

## Solution

```SQL
SELECT DISTINCT CITY
FROM STATION
WHERE CITY LIKE 'A%'
   OR CITY LIKE 'E%'
   OR CITY LIKE 'I%'
   OR CITY LIKE 'O%'
   OR CITY LIKE 'U%'
ORDER BY CITY ASC;
```