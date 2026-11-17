## Weather Observation Station 2


Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-2/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition


## Solution

```SQL
SELECT ROUND(SUM(LAT_N), 2), ROUND(SUM(LONG_W), 2)
FROM STATION;

```

