https://programmers.co.kr/learn/courses/30/lessons/59042  
  
   
   아우터조인의 기본적 지식을 묻는 문제.  
   
```SQL
SELECT A.ANIMAL_ID, A.NAME
from ANIMAL_OUTS A LEFT JOIN ANIMAL_INS B ON A.ANIMAL_ID = B.ANIMAL_ID
WHERE   B.ANIMAL_ID IS NULL
ORDER BY A.ANIMAL_ID, A.NAME
```
