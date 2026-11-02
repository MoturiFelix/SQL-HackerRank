## Weather Observation Station 8

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-8/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition

Pick City from Table Station. Where there is no repeated city. 
Only include cities that start and end with a vowel

## Solution

```SQL
SELECT DISTINCT CITY
FROM STATION
WHERE (CITY LIKE 'a%' OR CITY LIKE 'e%' OR CITY LIKE 'i%' OR CITY LIKE 'o%' OR CITY LIKE 'u%')
AND (CITY LIKE '%a' OR CITY LIKE '%e' OR CITY LIKE '%i' OR CITY LIKE '%o' OR CITY LIKE '%u');

```