*Type of Triangle*
------------------------------------------

```
SELECT
CASE
    WHEN (A+B<=C) OR (A+C<=B) or (B+C<=A) THEN 'Not A Triangle'
    WHEN A=B AND A=C THEN 'Equilateral'
    WHEN (A=B AND A<>C) OR (A=C AND B<>C) OR (B=C AND A<>C) THEN 'Isosceles'
    ELSE 'Scalene'
END
FROM TRIANGLES;
```