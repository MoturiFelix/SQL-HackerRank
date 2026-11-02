## Weather Observation Station 4

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-9/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition
Pick City from Table Station. Where there is no repeated city. 
Exclude alls cities that start with a vowel


## Solution

```SQL
SELECT DISTINCT CITY
FROM STATION
WHERE CITY NOT LIKE 'A%'
  AND CITY NOT LIKE 'E%'
  AND CITY NOT LIKE 'I%'
  AND CITY NOT LIKE 'O%'
  AND CITY NOT LIKE 'U%';

```