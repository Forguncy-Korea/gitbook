# QueryNullPolicy 열거형

### 설명&#x20;

데이터 테이블 또는 뷰 데이터를 가져올 때 null 값이 발생하는 정책입니다. [getTableDataByCondition](../forguncymethod/gettabledatabycondition.md) 메서드에 사용됩니다.

### 멤버&#x20;



| 멤버                            | 설명                      |
| ----------------------------- | ----------------------- |
| QueryAllItemsWhenValueIsNull  | 값이 비어 있으면 모든 항목이 쿼리됩니다. |
| QueryZeroItemsWhenValueIsNull | 값이 비어 있으면 0 항목을 쿼리합니다.  |
