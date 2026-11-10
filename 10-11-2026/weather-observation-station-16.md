## weather-observation-station-16

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-16/problem?isFullScreen=true)



DB Engine : MySQL

*********

## Intuition



## Solution

```SQL
SELECT ROUND(MIN(LAT_N), 4)
FROM STATION
WHERE LAT_N > 38.7780;
```