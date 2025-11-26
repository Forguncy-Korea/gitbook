# PivotTableEventParameter 클래스

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366308/blue%20block.png?version=1\&modificationDate=1648092745000\&api=v2) **설명입니다** <a href="#pivottableeventparameter-lei-miao-shu" id="pivottableeventparameter-lei-miao-shu"></a>

피벗 테이블 클릭 이벤트에 대한 데이터를 제공합니다.



#### ![](https://help.grapecity.com.cn/download/thumbnails/72366308/blue%20block.png?version=1\&modificationDate=1648092745000\&api=v2) **속** <a href="#pivottableeventparameter-lei-shu-xing" id="pivottableeventparameter-lei-shu-xing"></a>

| 속성         | 형식                                                  | 설명                                                                                   |
| ---------- | --------------------------------------------------- | ------------------------------------------------------------------------------------ |
| dataType   | string                                              | 클릭한 위치가 일반 데이터 범위인 경우 \[Data]이고 열 합계 셀의 경우 \[ColTotal]이고 행 합계 범위의 경우 \[RowTotal]입니다. |
| row        | number                                              | 클릭 위치의 행 인덱스입니다                                                                      |
| col        | number                                              | 위치의 열 인덱스를 클릭합니다.                                                                    |
| value      | any                                                 | 클릭 위치의 값입니다.                                                                         |
| colHeaders | [PivotTableHeaderInfo\[\]](pivottableheaderinfo.md) | 위치가 있는 열 헤더 정보를 클릭합니다.                                                               |
| rowHeaders | [PivotTableHeaderInfo\[\]](pivottableheaderinfo.md) | 위치가 있는 헤더 정보를 클릭합니다.                                                                 |
