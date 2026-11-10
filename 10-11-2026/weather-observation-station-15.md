## weather Observation Station-15

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-15/problem?isFullScreen=true)


DB Engine : MySQL

*********

## Intuition
We will need to create a subquery to get the maximum LAT_N below the specified upper limit. The outer query finds the corresponding LONG_W. Round the longitude to 4 decimal places.

## Solution

```SQL
SELECT ROUND(LONG_W, 4)
FROM STATION
WHERE LAT_N = (
    SELECT MAX(LAT_N)
    FROM STATION
    WHERE LAT_N < 137.2345
);

```