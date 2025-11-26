# ListviewPaginationInfo 인터페이스

리스트뷰의 페이징 정보를 나타냅니다. getPaginationInfo 메서드에 사용됩니다.

| 속성                   | 형식     | 설명                         |
| -------------------- | ------ | -------------------------- |
| MaxRowCountOfOnePage | number | 한 페이지에 표시되는 최대 행 수입니다.     |
| PageCount            | number | 페이지 수입니다.                  |
| PageIndex            | number | 현재 페이지의 인덱스입니다. 0부터 시작합니다. |
| TotalRowCount        | number | 총 행 수입니다.                  |
