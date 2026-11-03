## Weather Observation Station 12

Link: [Hackerrank](https://www.hackerrank.com/challenges/weather-observation-station-12/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition
Result should be based on two conditions. That is each output should  notr start with a vowel nor end with a vowel.


## Solution

```SQL
SELECT DISTINCT CITY
FROM STATION
WHERE CITY NOT LIKE 'A%'
  AND CITY NOT LIKE 'E%'
  AND CITY NOT LIKE 'I%'
  AND CITY NOT LIKE 'O%'
  AND CITY NOT LIKE 'U%'

AND CITY NOT LIKE '%A'
  AND CITY NOT LIKE '%E'
  AND CITY NOT LIKE '%I'
  AND CITY NOT LIKE '%O'
  AND CITY NOT LIKE '%U';

```