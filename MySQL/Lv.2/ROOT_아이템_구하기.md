문제 : [ROOT 아이템 구하기](https://school.programmers.co.kr/learn/courses/30/lessons/273710)

```sql
SELECT ITEM_INFO.ITEM_ID, ITEM_NAME
FROM ITEM_INFO
         JOIN ITEM_TREE
              ON ITEM_INFO.ITEM_ID = ITEM_TREE.ITEM_ID
WHERE ITEM_TREE.PARENT_ITEM_ID is null
ORDER BY ITEM_ID ASC
;
```