 ## Revising The Select Query 2

Link: [Hackerrank](https://www.hackerrank.com/challenges/revising-the-select-query-2/problem?isFullScreen=true)


Difficulty : Easy
DB Engine : MySQL

*********

## Intuition
Objective is to Query Names of Cities in USA that have a population greater than 120,000. 
I have selected Names from the City table With the country Code USA and Narrowed down the search to a population greater than 120,000

## Solution
```SQL
SELECT NAME FROM CITY WHERE COUNTRYCODE = 'USA' AND POPULATION > 120000;
```
