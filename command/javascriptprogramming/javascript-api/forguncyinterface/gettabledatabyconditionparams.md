# GetTableDataByConditionParams 인터페이스

데이터 테이블 또는 뷰 데이터를 가져올 때의 매개 변수입니다. getTableDataByCondition 메서드 에 사용합니다.



| 속성             | 형식                   | 설명                |
| -------------- | -------------------- | ----------------- |
| Columns        | string\[]            | 가져온 열의 이름 컬렉션입니다. |
| QueryCondition | object               | 정보를 쿼리합니다.        |
| QueryPolicy    | TableDataQueryPolicy | 쿼리할 때의 정책입니다.     |
| SortCondition  | object               | 정보를 정렬합니다.        |
| TableName      | string               | 테이블 또는 뷰의 이름입니다.  |
