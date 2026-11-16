## Weather-observation-station-18

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-18/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition

Get to know what is Manhattan distance = (x_2-x_1) + (y_2-y_1). 
Replace the quantities as described by Hacker rank. 

 a happens to equal the minimum value in Northern Latitude (LAT_N in STATION).
 b happens to equal the minimum value in Western Longitude (LONG_W in STATION).
 c happens to equal the maximum value in Northern Latitude (LAT_N in STATION).
 d happens to equal the maximum value in Western Longitude (LONG_W in STATION).
   

## Solution

```SQL

SELECT
    ROUND(
        (MAX(LAT_N) - MIN(LAT_N)) +
        (MAX(LONG_W) - MIN(LONG_W)),
        4
    )
FROM STATION;

```