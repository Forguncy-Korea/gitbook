# TreeSelect

TreeSelect는 트리구조의 항목을 선택하여 사용할 수 있는 셀타입입니다.

### 빌더화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (1200).png" alt=""><figcaption></figcaption></figure>



### 실행화면 (런타임)

<figure><img src="../../../../.gitbook/assets/image (1771).png" alt=""><figcaption></figcaption></figure>



### 셀속성&#x20;

<table><thead><tr><th width="241">이름</th><th>설명 </th></tr></thead><tbody><tr><td>명령 편집</td><td>값이 변경될 때 실행할 명령 구성</td></tr><tr><td>데이터 유효성 검사</td><td>셀의 구성 데이터 유효성 검사, 업데이트 명령 실행 또는 요청 서버 명령 실행 시에만 유효성 검사</td></tr><tr><td>UI 권한편집 </td><td>현재 사용자의 역할에 따라 권한 표시/활성화</td></tr><tr><td>기본값 </td><td> TreeSelect의 기본값 </td></tr><tr><td>데이터연동 </td><td>항목이 데이터베이스에서 바인딩되는지 여부를 나타냅니다. <img src="../../../../.gitbook/assets/image (1709).png" alt=""></td></tr><tr><td>항목 구성 </td><td>디자인 타임에 바인딩 해제 항목 구성</td></tr><tr><td>입력 안내 </td><td>텍스트가 비어 있을 때만 표시</td></tr><tr><td>다수 선택 모드 </td><td>여러 항목 선택 허용 여부</td></tr><tr><td>트리 옵션</td><td>다중이 참인 경우에만 사용 가능</td></tr><tr><td>선택된 상하위 노드를 지속 표시</td><td>리프 노드만 선택하거나 아무 노드나 선택할 수 있습니다.</td></tr><tr><td>항목 검색 기능</td><td>항목을 검색하기 위해 일부 키워드 입력 허용</td></tr><tr><td>선택 후 지우기 버튼 표시</td><td>지우기 허용</td></tr><tr><td>비활성화</td><td>TreeSelect 비활성화</td></tr></tbody></table>

### 트리옵션&#x20;

<figure><img src="../../../../.gitbook/assets/image (1681).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="284">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>Indent</td><td>인접한 레벨의 노드 가로 들여쓰기(픽셀 단위)</td></tr><tr><td>HighlightCurrent</td><td>현재 노드가 강조 표시되는지 여부</td></tr><tr><td>DefaultExpandAll</td><td>기본적으로 모든 노드를 확장할지 여부</td></tr><tr><td>ExpandOnClickNode</td><td>노드를 클릭할 때 노드를 확장하거나 축소할지 여부, false인 경우 화살표 아이콘을 클릭할 때만 노드를 확장하거나 축소합니다.</td></tr><tr><td>AutoExpandParent</td><td>자식 노드 확장 시 아버지 노드 확장 여부</td></tr><tr><td>Accordion</td><td>한 번에 같은 수준의 노드 하나만 확장할 수 있는지 여부</td></tr><tr><td>ShowCheckBox</td><td>노드 선택 가능 여부</td></tr></tbody></table>

### 관련 명령 빠른 생성&#x20;

| 데이터 소스 설정 (객체 트리)   | <p>동적 JSON 객체 트리를 셀의 데이터 소스로 사용하는 JSON 형식의 예는 다음과 같습니다.<br>[<br>    {<br>        "value": 1,<br>        "label": "Department1",<br>        "children": [<br>            {<br>                "value": 2,<br>                " label": "Sub-department1"<br>            },<br>            {<br>                "value": 3,<br>                "label": "Sub-department2",<br>                "children": [<br>                    {<br>                       "value": 4,<br>                       "label":"하위 부서2-1"<br>                    }<br>                ]<br>            }<br>        ]<br>    },<br>    {<br>        "value": 5,<br>        "label": "Department2"<br>    },<br>    {<br>        "value": 6,<br>        "label": "Department3"<br>    }<br>]<br>위의 데이터는 'value attribute'가 value, 'label attribute name'이 값이라고 가정합니다. 는 레이블이고 '자식 속성 이름'은 '자식'입니다<br>. 일반적으로 JSON 데이터 소스는 HTTP 요청 명령을 통해 웹 서비스에서 또는 서버측 명령에서 가져올 수 있습니다.</p> |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 데이터 소스 설정 (2차원 테이블) | <p>테이블 JSON 객체 트리를 셀의 데이터 소스로 사용하는 JSON 형식 예제는<br>[<br>    {"value": 1, "label": "Department1", "parentValue": null},<br>    {"value": 2, "label": "Department1-1", "parentValue": 1},<br>    {"value": 3, "label": "Department1-2", "parentValue": 1},<br>    {"value": 4, "label" ": "Department1-2-1", "parentValue": 3},<br>    {"value": 5, "label": "Department2", "parentValue": null},<br>    {"value": 6, "label": "부서3", "부모값":null}<br>]<br>위의 데이터는 'value 속성'을 value, 'label 속성명'을 label, '상위값 속성명'을 'parentValue'로 가정하고 있다<br>. 데이터베이스</p>                                                                                                                                                                                                                                                                                                                                                                                                 |
| 연동 데이터 새로고침         | <p> 데이터  연동에서만 사용 가능<br> 바인딩이 변경되었지만 바인딩 항목이 데이터를 자동으로 다시 로드할 수 없는 경우 이 작업을 사용하면 바인딩 항목을 강제로 다시 로드할 수 있습니다.</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
