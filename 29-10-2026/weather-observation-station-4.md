## Weather Observation Station 4

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-4/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition

Retrieve the total number of cities in the STATION table, count the unique cities without duplicates, and calculate the difference between the two counts.

## Solution

```SQL
SELECT COUNT(CITY) - COUNT(DISTINCT CITY)
FROM STATION;
```