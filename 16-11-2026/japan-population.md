### Japan Population


Link: [Hackerrank](https://www.hackerrank.com/challenges/japan-population/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition

Query the sum of the populations for all Japanese cities in CITY using COUNTRYCODE for Japan as JPN.

## Solution

```SQL

SELECT SUM(POPULATION)
FROM CITY
WHERE COUNTRYCODE = 'JPN';

```