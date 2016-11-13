Show the countries which have a name that includes the word 'United'

select name 
from world 
where name LIKE 'United%'

 Select the code which shows the countries that end in A or L
 
 SELECT name FROM world
 WHERE name LIKE '%a' OR name LIKE '%l'
 
 Exclusive OR (XOR). Show the countries that are big by area or big by population but not both. Show name, population and area.
 
 select name, population, area 
from world 
where area > 3000000 xor population > 250000000

Show the name and per-capita GDP for those countries with a GDP of at least one trillion (1000000000000; that is 12 zeros). Round this value to the nearest 1000.

select name, ROUND(gdp/population,-3)
from world 
where gdp >= 1000000000000

Select the code which would give two rows

ELECT name FROM world
 WHERE name IN ('Cuba', 'Togo')
