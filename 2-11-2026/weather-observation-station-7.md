## Weather Observation Station 7

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-7/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition

Pick City from Table Station. Where there is no repeated city. 
Only include cities that end with a vowel

## Solution

```SQL
SELECT DISTINCT CITY
FROM STATION
WHERE CITY LIKE '%a'
   OR CITY LIKE '%e'
   OR CITY LIKE '%i'
   OR CITY LIKE '%o'
   OR CITY LIKE '%u';

```