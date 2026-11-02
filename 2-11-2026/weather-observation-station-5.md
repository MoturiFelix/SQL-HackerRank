## Weather Observation Station 5

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-5/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition

The question has two sides. First get the City with the least characters. Then second get the city with the longest number of characters. 
For both make sure you have only one result for each query. 

For both make sure you follow the order. 

## Solution

```SQL
(SELECT CITY, LENGTH(CITY)
FROM STATION
ORDER BY LENGTH(CITY) ASC, CITY ASC
LIMIT 1
)
UNION ALL
(
SELECT CITY, LENGTH(CITY)
FROM STATION
ORDER BY LENGTH(CITY) DESC, CITY ASC
LIMIT 1
);

```