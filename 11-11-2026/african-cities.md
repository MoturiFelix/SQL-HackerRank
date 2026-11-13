## African Cities

## What type of Triangle

Link: [Hackerrank](https://www.hackerrank.com/challenges/african-cities/problem?isFullScreen=true)


Difficulty : Medium
DB Engine : MySQL

*********

## Intuition
InnerJoin the twpo tables to piuck data from each



## Solution

```SQL
SELECT CITY.NAME
FROM CITY
INNER JOIN COUNTRY
    ON CITY.COUNTRYCODE = COUNTRY.CODE
WHERE COUNTRY.CONTINENT = 'Africa';

```