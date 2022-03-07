https://programmers.co.kr/learn/courses/30/lessons/59405
ROWNUM을 활용해야 풀 수 있는 문제.
여기서 ROWNUM은 WHERE 절에서 수행하므로 ORDER BY 보다 먼저 수행되기 때문에 FROM 절에서 정렬 후 수행해야한다.
  
  

```sql
SELECT  NAME
FROM (
SELECT  NAME
FROM    ANIMAL_INS
ORDER BY DATETIME)
WHERE ROWNUM = 1
```
