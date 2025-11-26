# ModifyData 인터페이스

리스트뷰의 변경을 나타내는 행 데이터입니다. modifyTablesData 메서드에 사용됩니다.



| 속성         | 형식                                                   | 설명        |
| ---------- | ---------------------------------------------------- | --------- |
| addRows    | \[columnName: string]: Object                        | 추가된 행입니다. |
| deleteRows | primaryKey: { \[primaryColumnName: string]: Object } | 삭제된 행입니다. |
| editRows   | primaryKey: { \[primaryColumnName: string]: Object } | 편집된 행입니다. |
