# TableDataQueryPolicy 인터페이스

&#x20; 데이터 테이블 또는 뷰 데이터를 가져올 때의 정책입니다. getTableDataByCondition 메서드에 사용됩니다.

| 속성              | 형식              | 설명                                               |
| --------------- | --------------- | ------------------------------------------------ |
| Distinct        | boolean         | 다른 결과가 있는지 여부.                                   |
| QueryNullPolicy | QueryNullPolicy | 쿼리 값이 비어 있는 경우 쿼리 정책입니다.                         |
| IgnoreCache     | boolean         | 캐시를 무시할지 여부는 기본적으로 사이트가 포스트 매개 변수에 따라 결과를 캐시합니다. |
