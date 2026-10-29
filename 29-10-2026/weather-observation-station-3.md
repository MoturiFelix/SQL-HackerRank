## Weather Observation Station 3

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-3/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition

Retrieve a list of city names from the STATION table where the ID is an even number. Exclude duplicate city names.
## Solution

```SQL
SELECT DISTINCT CITY
FROM STATION
WHERE MOD(ID, 2) = 0;
```