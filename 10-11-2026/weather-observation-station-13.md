## Weather Observation Station 13

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-13/problem?isFullScreen=true)


DB Engine : MySQL

*********

## Intuition
Condition is that the sum should be for Data in Northern Latitude greater than 38.7880 and less than 137.2345. Th Make the result in 4 decimal places. 


## Solution

```SQL
SELECT ROUND(SUM(LAT_N), 4)
FROM STATION
WHERE LAT_N > 38.7880
  AND LAT_N < 137.2345;

```