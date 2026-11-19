## Asian Population

Link: [Hackerrank](https://www.hackerrank.com/challenges/asian-population/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition


## Solution

```SQL

SELECT SUM(CITY.POPULATION)
FROM CITY
INNER JOIN COUNTRY
    ON CITY.COUNTRYCODE = COUNTRY.CODE
Where COUNTRY.CONTINENT = 'ASIA';

```