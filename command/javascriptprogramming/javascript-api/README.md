# JavaScript API 인덱스

일부 속성, 메서드, 인터페이스, 조작 가능한 페이지 개체, 리스트뷰 개체 및 셀 개체 등이 제공됩니다.

#### 네임스페이스  <a href="#javascriptapi-suo-yin-ming-ming-kong-jian" id="javascriptapi-suo-yin-ming-ming-kong-jian"></a>

Forguncy

#### 메서드&#x20;



| 메서드                                                                           | 설명                                                                                                              |
| ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| [addTableData](forguncymethod/addtabledata.md)                                | 이 메서드를 사용 하 여 지정 된 데이터 테이블에 대 한 데이터를 추가 합니다.                                                                    |
| [addUserToRole](forguncymethod/addusertorole.md)                              | 이 메서드를 사용 하 여 지정 된 그룹에 지정 된 사용자를 추가 하 여 사용자에 대 한 역할을 지정 합니다.                                                    |
| [addUser](forguncymethod/adduser.md)                                          | 이 방법을 사용하여 일반 인증 모드를 포함하여 사용자를 추가하고 도메인 인증 모드에서 사용자를 추가합니다.                                                     |
| [ConvertDateToOADate](forguncymethod/convertdatetooadate.md)                  | 이 메서드를 사용 하 여 DateTime을 OADate로 변환 합니다.                                                                         |
| [ConvertOADateToDate](forguncymethod/convertoadatetodate.md)                  | 이 메서드를 사용 하 여 OADATE에서 DateTime으로 변환 합니다.                                                                       |
| [ConvertToCssColor](forguncymethod/converttocsscolor.md)                      | 지정된 색상 텍스트를 CSS 색상 텍스트, 즉 색상의 16진수 값으로 변환합니다.                                                                   |
| [deleteTableData](forguncymethod/deletetabledata.md)                          | primaryKey 매개 변수를 통해 지정된 고유 레코드를 삭제합니다.                                                                         |
| [deleteUserFromRole](forguncymethod/deleteuserfromrole.md)                    | 이 메서드를 사용 하 여 지정 된 그룹에서 지정 된 사용자를 제거 합니다.                                                                       |
| [deleteUser](forguncymethod/deleteuser.md)                                    | 이 메서드를 사용 하 여 지정 된 사용자를 제거 합니다.                                                                                 |
| [forceSyncTableData](forguncymethod/forcesynctabledata.md)                    | 아웃리치 테이블의 데이터를 복제본 테이블에 강제로 동기화합니다.                                                                             |
| [getTableDataByCondition](forguncyinterface/gettabledatabyconditionparams.md) | 조건을 통해 데이터 테이블 또는 뷰에 대한 데이터를 가져옵니다.                                                                             |
| [getTableDataByOData](forguncymethod/gettabledatabyodata.md)                  | OData 쿼리 문자열을 통해 데이터를 가져옵니다.                                                                                    |
| [getTableData](forguncymethod/gettabledata.md)                                | 데이터베이스의 기본 키를 사용하여 데이터 테이블의 레코드를 가져옵니다.                                                                         |
| [logIn](forguncymethod/login.md)                                              | 이 메서드를 사용 하 여 지정 된 사용자 이름 및 암호와 연결 된 계정에 로그인 합니다.                                                               |
| [logOut](forguncymethod/logout.md)                                            | 이 메서드를 사용 하 여 현재 사용자를 로그 아웃 합니다.                                                                                |
| [modifyTablesData](forguncymethod/modifytablesdata.md)                        | 데이터 테이블의 데이터를 추가, 수정 및 삭제합니다.                                                                                   |
| [SendMail](forguncymethod/sendmail.md)                                        | 지정된 이메일 주소로 제목과 콘텐츠를 지정하는 이메일을 보내고 발신자는 현재 웹 사이트에 로그인한 사용자입니다. 이 API를 사용하여 전자 메일을 보내려면 SMTP 서비스를 올바르게 구성해야 합니다. |
| [updateTableData](forguncymethod/updatetabledata.md)                          | primaryKey 매개 변수를 사용하여 업데이트할 레코드의 고유한 행을 지정합니다.                                                                 |

#### 클래스&#x20;



| 클래스                             | 설명                             |
| ------------------------------- | ------------------------------ |
| [Cell](class/cellclass/)        | 셀 개체입니다.                       |
| [CellEvents](class/cellevents/) | 셀에서 지원하는 이벤트입니다.               |
| Page                            | 페이지 개체입니다.                     |
| Helper                          | 몇 가지 도움말 메서드를 제공하는 도움말 클래스입니다. |
| [ListView](class/listview/)     | 테이블 개체입니다.                     |
| ListViewEvents                  | 테이블에서 지원하는 이벤트입니다.             |
| PageEvents                      | 페이지에서 지원되는 이벤트입니다.             |
| SpecialPath                     | 특수 경로입니다.                      |
| PivotTableCellType              | 피벗 테이블 셀 유형입니다.                |

#### 인터페이스&#x20;



| 인터페이스                                                                               | 설명                                 |
| ----------------------------------------------------------------------------------- | ---------------------------------- |
| [CellLocationInfo](forguncyinterface/celllocationinfo.md)                           | 셀의 위치 정보입니다.                       |
| [CellRange](forguncyinterface/cellrange.md)                                         | 셀 범위의 위치 정보입니다.                    |
| [CurrentRowInfoParam](forguncyinterface/currentrowinfoparam.md)                     | 현재 행 매개 변수에 대한 정보입니다.              |
| [FormulaCalcContext](forguncyinterface/formulacalccontext.md)                       | 수식 계산에 대한 컨텍스트 정보입니다.              |
| [GetTableDataByConditionParams](forguncyinterface/gettabledatabyconditionparams.md) | 데이터 테이블 또는 뷰 데이터를 가져올 때의 매개 변수입니다. |
| [IMergedColumnInfo](forguncyinterface/imergedcolumninfo.md)                         | 테이블의 열 정보를 나타냅니다.                  |
| [ListviewPaginationInfo](forguncyinterface/listviewpaginationinfo.md)               | 테이블의 페이징 정보를 나타냅니다.                |
| [ListViewValueChangedEventArg](forguncyinterface/listviewvaluechangedeventarg.md)   | 테이블 값 변경 이벤트에 대한 데이터를 제공합니다.       |
| [ModifyData](forguncyinterface/modifydata.md)                                       | 테이블의 변경을 나타내는 행 데이터입니다.            |
| [OrganizationLevelValueInfo](forguncyinterface/organizationlevelvalueinfo.md)       | 사용자의 조직 수준 정보입니다.                  |
| [RowData](forguncyinterface/rowdata.md)                                             | 테이블의 행 데이터를 나타내는 정보입니다.            |
| [TableDataQueryPolicy](forguncyinterface/tabledataquerypolicy.md)                   | 데이터 테이블 또는 뷰 데이터를 가져올 때의 정책입니다.    |
| [UserExtendProperties](forguncyinterface/userextendproperties.md)                   | 사용자의 사용자 지정 속성입니다.                 |
| [UserInfo](forguncyinterface/userinfo.md)                                           | 사용자에 대한 정보입니다.                     |

#### 열거형&#x20;

| 열거형                                                  | 설명                                          |
| ---------------------------------------------------- | ------------------------------------------- |
| [ListviewColumnType](forguncy/listviewcolumntype.md) | 테이블의 열 유형을 나타냅니다.                           |
| [QueryNullPolicy](forguncy/querynullpolicy.md)       | 데이터 테이블 또는 뷰 데이터를 가져올 때 null 값이 발생하는 정책입니다. |
