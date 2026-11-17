## Earnings-of-employees


Link: [Hackerrank](https://www.hackerrank.com/challenges/earnings-of-employees/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition
Get the sum of all data in LAT_N and LONG_W. Round each of the nearest 2 decimals. 

## Solution

```SQL
SELECT ROUND(SUM(LAT_N), 2), ROUND(SUM(LONG_W), 2)
FROM STATION;

```

