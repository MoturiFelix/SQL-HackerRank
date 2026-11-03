## Weather Observation Station 10

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-10/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition
Result should have the output as List of CITY names that do not end with Vowels. 
No Duplicates.



## Solution

```SQL
SELECT DISTINCT CITY
FROM STATION
WHERE CITY NOT LIKE '%A'
  AND CITY NOT LIKE '%E'
  AND CITY NOT LIKE '%I'
  AND CITY NOT LIKE '%O'
  AND CITY NOT LIKE '%U';

```