# ListView 클래스

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365388/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 설명 <a href="#listview-lei-miao-shu" id="listview-lei-miao-shu"></a>

리스트뷰 개체입니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365388/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 메서드 <a href="#listview-lei-fang-fa" id="listview-lei-fang-fa"></a>

| 메서드                                                   | 설명                                                                                                                                                           |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [addNewRow](addnewrow.md)                             | 리스트뷰에 새 행에 대한 데이터를 포함하여 새 행을 추가합니다.                                                                                                                          |
| [addSelectedRow](addselectedrow.md)                   | 리스트뷰에서 지정된 행을 선택합니다. 리스트뷰 여러 번 선택할 수 있는 경우 행을 선택한 후 이 메서드를 사용하여 지정된 행을 하나 더 선택할 수 있습니다. 테이블에서 라디오만 허용하는 경우 행을 선택한 다음 이 메서드를 사용하여 지정된 행을 선택하고 이전 행은 선택 취소합니다. |
| [bind](../cellclass/bind.md)                          | 선택한 리스트뷰에 하나 이상의 이벤트 처리기를 추가하고 이벤트가 발생할 때 실행되는 함수를 지정합니다.                                                                                                    |
| [clearAllSelectedRows](clearallselectedrows.md)       | 리스트뷰에서 선택한 모든 행의 선택을 취소합니다.                                                                                                                                  |
| [clearSelectedRowByQuery](clearselectedrowbyquery.md) | 쿼리 조건에 따라 리스트뷰의 선택 행을 지웁니다.                                                                                                                                  |
| [clearSelectedRow](clearselectedrow.md)               | 리스트뷰에 지정된 선택 행의 선택을 취소합니다.                                                                                                                                   |
| [deleteRow](deleterow.md)                             | 리스트뷰에 지정된 행을 삭제합니다.                                                                                                                                          |
| [getDataTableName](getdatatablename.md)               | 리스트뷰가 바인딩된 데이터 테이블 또는 뷰의 이름을 가져옵니다.                                                                                                                          |
| [getDesignerRangeInfo](getdesignerrangeinfo.md)       | 시작 행 인덱스, 시작 열 인덱스, 테이블 행 수 및 열 수를 포함하여 디자이너에서 리스트뷰 위치 정보를 가져옵니다.                                                                                            |
| [getMergedColumnInfos](getmergedcolumninfos.md)       | 리스트뷰의 모든 열에 대한 정보를 가져옵니다. 행 헤더 열, 선택 열, 숨겨진 열 등을 포함합니다.                                                                                                      |
| [getName](getname.md)                                 | 리스트뷰의 이름을 가져옵니다.                                                                                                                                             |
| [getPaginationInfo](getpaginationinfo.md)             | 리스트뷰 페이지 번호 정보를 가져옵니다. 리스트뷰에 페이징이 없는 경우 반환 값은 null이 됩니다.                                                                                                     |
| [getQuery](getquery.md)                               | 지정된 행의 기본 키를 가져옵니다.                                                                                                                                          |
| [getRowCount](getrowcount.md)                         | 리스트뷰의 행 수를 가져옵니다.                                                                                                                                            |
| [getSelectedRowIndex](getselectedrowindexs.md)        | 선택한 행의 행 인덱스를 가져옵니다. 행 인덱스는 0부터 시작합니다.                                                                                                                       |
| [getSelectedRowIndexs](getselectedrowindex.md)        | 선택한 행의 행 인덱스를 가져옵니다. 여러 행을 선택하면 선택한 모든 행의 행 인덱스가 포함된 배열이 반환됩니다. 행 인덱스는 0부터 시작합니다.                                                                            |
| [getSelectedRowsData](getselectedrowsdata.md)         | 리스트뷰 선택 행에 대한 데이터를 가져옵니다. 여기에는 행의 행 인덱스, 쿼리 조건 및 데이터 선택이 포함됩니다.                                                                                              |
| [getText](gettext.md)                                 | <p>리스트뷰의 지정된 셀에 있는 텍스트를 가져옵니다.<br></p>                                                                                                                       |
| [getValue](getvalue.md)                               | 리스트뷰의 지정된 위치에 있는 셀의 값을 가져옵니다.                                                                                                                                |
| [goToFirstPage](gotofirstpage.md)                     | 리스트뷰 페이지 매김 탐색 버튼을 사용하여 테이블 데이터를 페이징하는 경우 이 방법을 사용하면 리스트뷰의 첫 번째 페이지로 이동하여 첫 번째 페이지의 데이터를 표시할 수 있습니다.                                                         |
| [goToLastPage](gotolastpage.md)                       | 리스트뷰이 페이지 매김 탐색 버튼을 사용하여 테이블 데이터를 페이징하는 경우 이 방법을 사용하면 테이블이 마지막 페이지로 이동하여 마지막 페이지의 데이터를 표시할 수 있습니다.                                                           |
| [goToNextPage](gotonextpage.md)                       | 리스트뷰 페이지 매김 탐색 버튼 사용하여 테이블 데이터를 페이징하는 경우 이 방법을 사용하면 테이블이 현재 페이지의 다음 페이지로 이동하여 다음 페이지의 데이터를 표시할 수 있습니다.                                                       |
| [goToPreviousPage](gotopreviouspage.md)               | 리스트뷰 페이지 매김 탐색 버튼을  사용하여 테이블 데이터를 페이징하는 경우 이 방법을 사용하면 테이블이 현재 페이지의 이전 페이지로 이동하여 이전 페이지의 데이터를 표시할 수 있습니다.                                                     |
| [goToSpecifiedPage](gotospecifiedpage.md)             | 리스트뷰 페이지 매김 탐색 버튼을 사용하여 테이블 데이터를 페이징하는 경우 이 방법을 사용하면 테이블이 지정된 페이지로 이동하여 지정된 페이지의 데이터를 표시할 수 있습니다.                                                            |
| [hideColumns](hidecolumns.md)                         | 리스트뷰의 열을 숨깁니다.                                                                                                                                               |
| [hiddenLoadingIndicator](hiddenloadingindicator.md)   | 리스트뷰의 로드 아이콘을 숨기고 리스트뷰의 정상적인 사용을 복원합니다. 일반적으로 [showLoadingIndicator](showloadingindicator.md) 메서드와 함께 사용됩니다.                                                 |
| [isSelectedRow](isselectedrow.md)                     | 지정된 행이 선택되었는지 여부를 가져옵니다. 반환 값은 true 또는 false입니다. true는 선택되고 false는 선택되지 않습니다.                                                                                |
| [reload](reload.md)                                   | 데이터베이스에서 데이터를 다시 로드합니다.                                                                                                                                      |
| [selectAllRows](selectallrows.md)                     | 리스트뷰의 모든 행을 선택합니다.                                                                                                                                           |
| [selectRow](selectrow.md)                             | 리스트뷰에 지정된 행을 현재 행으로 설정합니다.                                                                                                                                   |
| [setText](settext.md)                                 | 리스트뷰의 지정된 위치에 있는 셀의 텍스트를 설정합니다.                                                                                                                              |
| [setValue](setvalue.md)                               | 리스트뷰의 위치를 지정하는 셀에 대한 값을 설정합니다.                                                                                                                               |
| [showLoadingIndicator](showloadingindicator.md)       | 리스트뷰 로드 아이콘을 표시하고 [hiddenLoadingIndicator](hiddenloadingindicator.md)가 호출될 때까지 테이블을 비활성화합니다. 일반적으로 예기치 않은 작업을 방지하기 위해 리스트뷰을 조작하기 전에 많은 작업을 수행하는 데 사용됩니다.     |
| [showColumns](showcolumns.md)                         | API 및 열 옵션 명령을 통해 숨겨진 리스트뷰의 열을 표시합니다.                                                                                                                        |
| [unbind](unbind.md)                                   | 선택한 리스트뷰에 대한 이벤트 처리기를 제거합니다. 이 메서드는 선택한 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.                                                                    |
| [unbindAll](../cellclass/unbindall.md)                | 페이지 리스트뷰의 모든 이벤트에 대한 바인딩을 제거합니다. 이 메서드는 페이지 테이블의 모든 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.                                                        |
| [usePaginationDisplay](usepaginationdisplay.md)       | 이 메서드를 사용 하 여 리스트뷰에 데이터를 페이징 하 고 페이지 당 표시할 행 수를 설정 하 고 지정 된 페이지 번호로 이동할 수 있습니다.                                                                              |
| [clearAllColumnFilters](clearallcolumnfilters.md)     | 리스트뷰의 모든 열 필터 항목을 지웁니다.                                                                                                                                      |
| [getRunTimePageName](getruntimepagename.md)           | 리스트뷰가 있는 런타임 페이지의 이름을 가져옵니다.                                                                                                                                 |
