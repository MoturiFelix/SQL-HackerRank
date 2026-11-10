## Weather-observation-station-14

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-14/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition
One Condition which is the result should be less than 137.2345b in Northern Latitude. 
There should also be one result which is the maximum number and truncated to 4 decimal places. 


## Solution

```SQL
SELECT TRUNCATE(MAX(LAT_N), 4)
FROM STATION
WHERE LAT_N < 137.2345;

```