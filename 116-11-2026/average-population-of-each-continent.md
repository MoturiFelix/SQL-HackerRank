## Average-Population-of-Each-Continent

Link: [Hackerrank](https://www.hackerrank.com/challenges/average-population-of-each-continent/problem?isFullScreen=true)


DB Engine : MySQL

*********

## Intuition

JOin both tables( Country and City). CITY.CountryCode and COUNTRY.Code are matching key columns. . look for all cities from the continet Asia. Get the sum of the population from all the Asia - Cities


## Solution

```SQL
SELECT
    COUNTRY.CONTINENT,
    FLOOR(AVG(CITY.POPULATION))
FROM CITY
INNER JOIN COUNTRY
    ON CITY.COUNTRYCODE = COUNTRY.CODE
GROUP BY COUNTRY.CONTINENT;

```