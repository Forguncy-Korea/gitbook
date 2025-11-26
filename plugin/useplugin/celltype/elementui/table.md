# 표

데이터를 표에 표현할 수 있는 셀타입입니다.  데이터테이블을 연결하여 사용할 수 있습니다.&#x20;



### 빌더화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (409).png" alt=""><figcaption></figcaption></figure>

### 실행화면 (런타임)

<figure><img src="../../../../.gitbook/assets/image (1831).png" alt=""><figcaption></figcaption></figure>

### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (518).png" alt=""><figcaption></figcaption></figure>



<table><thead><tr><th width="239">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>요소 표 이름 </td><td>표의 이름 </td></tr><tr><td>행클릭 명령 </td><td>표의 행 클릭 시 명령 </td></tr><tr><td>행 두번 클릭 명령 </td><td>표의 행을 두  번 클릭 시 명령 </td></tr><tr><td>현재 행 변경됨 명령 </td><td>표에서 현재 행이 바뀌었을 때의 명령 </td></tr><tr><td>Edit Selection Changed 명령 </td><td>표에서 현재 행이 바뀌었을 때의 명령 </td></tr><tr><td>데이터 소스 </td><td>표에서 사용할 데이터 소스를 설정 </td></tr><tr><td>데이터 소스별 열 자동생성 </td><td>설정한 데이터 소스를 표에서 자동으로 생성하는지의 여부 </td></tr><tr><td>수동으로 열 구성 </td><td><p>"데이터 소스에 의해 자동으로 열 생성" 옵션이 선택되지 않은 경우에만 작동합니다. 이 옵션은 일부 열 구성을 수동으로 수행하는 데 사용되며 설정은 다음과 같습니다.</p><ul><li>열 이름: 표시된 열 머리글 제목입니다.</li><li>데이터 소스의 열 이름: 로드하려는 데이터 소스의 열 데이터를 지정합니다.</li><li>서식 문자열: 날짜 유형 값을 일반 시간 문자열로 형식화합니다. 사용 가능한 옵션은 "yyyy/MM/dd" 및 "HH:mm"입니다.</li><li>열 너비: 테이블 열 머리글 포함.</li><li>열 최소 너비: 테이블 열 머리글 최소 너비입니다.</li><li>열 맞춤: 콘텐츠 정렬.</li><li>열 헤더 맞춤: 머리글 정렬.</li><li>정렬 활성화: 백엔드 정렬.</li><li>데이터 필터 활성화: 프런트 엔드 필터, 현재 페이지에만 적용됩니다.</li><li>다중 필터: 필터는 다중일 수 있습니다.</li><li>열 크기 조정 가능</li><li>오버플로 도구 설명 표시: 테이블 셀 내용이 너무 많아 포함할 수 없을 때 툴팁을 표시합니다.</li></ul></td></tr><tr><td>작업버튼표시 </td><td>테이블 열 끝에 작업 열을 추가할지 여부입니다. </td></tr><tr><td>작업 버튼 구성 </td><td>작업버튼표시를 체크해야 표시됨, 작업버튼의 유형과 이름, 스타일, 명령편집을 설정</td></tr><tr><td>작업 열의 너비 </td><td>작업 열의 너비 </td></tr><tr><td>푸터의 요약 표시 </td><td>푸터의 요약 표시를 체크하면 표 하단에 요약이 나옴 </td></tr><tr><td>요약 텍스트 </td><td>푸터의 요약 표시를 체크해야 표시되며, 요약의 텍스트를 나타냄</td></tr><tr><td>표 크기 </td><td>표의 크기를 대,중,소로 설정할 수 있음 </td></tr><tr><td>표 헤더 표시 </td><td>표 헤더를 표시할 지 여부 </td></tr><tr><td>인덱스 열 표시 </td><td>인덱스 열을 표시할 지 여부 </td></tr><tr><td>열 선택 표시 </td><td>열을 선택할 지 여부 </td></tr><tr><td>열 너비 자동 맞춤 </td><td>열을 자동으로 맞출 지 여부 </td></tr><tr><td>세로 테두리 </td><td>세로 테두리를 사용할 지 여부 </td></tr><tr><td>줄무늬 </td><td>줄무늬를 사용할 지 여부 </td></tr></tbody></table>



### 관련 명령 빠른 생성&#x20;

<table><thead><tr><th width="265">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>Config Column Properties</td><td>일반적으로 Json을 데이터 소스로 설정한 후 사용되는 기존 Column의 설정을 업데이트합니다.</td></tr><tr><td>선택 항목 지우기</td><td>선택한 항목을 지울 수 있는 명령 </td></tr><tr><td>현재 행 설정</td><td>현재행을 지정한 행인덱스로 설정하는 명령 </td></tr><tr><td>선택한 행 가져오기 </td><td>선택한 행을 가져오는 명령 </td></tr><tr><td>표 다시 설정 </td><td>표를 다시 설정하는 명령 </td></tr><tr><td>Json 데이터 소스 설정</td><td><p>동적 JSON 문자열 배열을 셀의 데이터 소스로 사용하는 경우 json 형식 예는 다음과 같습니다. </p><p>[ </p><p>{ "ID": 1, "Column": "Column content" },</p><p> { "ID": 2, "Column": "Column content" }, </p><p>{ "ID": 3, "Column": "Column content" } </p><p>] </p><p>일반적으로 데이터 소스는 HTTP 요청 명령을 통해 웹 서비스에서 얻거나 서버 측 명령을 통해 얻을 수 있습니다.</p></td></tr></tbody></table>
