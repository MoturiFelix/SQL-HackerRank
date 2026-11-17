## Japan City Names


Link: [Hackerrank](https://www.hackerrank.com/challenges/japanese-cities-name/problem?isFullScreen=true)

DB Engine : MySQL

*********

## Intuition

Select all names from the countrycode JPN 'japan'


## Solution

```SQL
SELECT NAME FROM CITY
WHERE COUNTRYCODE = 'JPN';
```

