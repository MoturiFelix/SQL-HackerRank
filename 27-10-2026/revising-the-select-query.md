
## Revising The Select Query

Link: [Hackerrank](https://www.hackerrank.com/challenges/revising-the-select-query/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition
Objective is to Query all Cities in USA that have a population greater than 100,000. 
I have selected all data from the City table With the country Code USA and Narrowed down the search to a population greater than 100,000

## Solution
```SQL
SELECT * FROM CITY WHERE CountryCode = 'USA' AND Population > 100000;
```

