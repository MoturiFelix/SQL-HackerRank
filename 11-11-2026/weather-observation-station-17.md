## weather-observation-station-17

## What type of Triangle

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-17/problem?isFullScreen=true)


DB Engine : MySQL

*********

## Intuition
We will need to create a subquery to get the minimum LAT_N below the specified limit. The outer query finds the corresponding LONG_W. Round the longitude to 4 decimal places.


## Solution

```SQL

SELECT ROUND(LONG_W, 4)
FROM STATION

WHERE LAT_N = (
    SELECT MIN(LAT_N)
    FROM STATION
    WHERE LAT_N > 38.7780
);

```