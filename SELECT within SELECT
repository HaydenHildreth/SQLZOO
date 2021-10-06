-- 1. Bigger than Russia

SELECT name FROM world
  WHERE population >
     (SELECT population FROM world
      WHERE name='Russia')
      
-- 2. Richer than UK

SELECT name
FROM world
WHERE continent='Europe' AND ((gdp/population)>(2471600000000/64105700));

-- 3. Neighbours of Argentina and Australia

SELECT name, continent
FROM world
WHERE continent='South America' OR continent='Oceania'
ORDER BY name ASC;

-- 4. Between Canada and Poland

SELECT name, population
FROM world
WHERE population<(SELECT population FROM world WHERE name='Poland') AND population>(SELECT population FROM world WHERE name='Canada');
