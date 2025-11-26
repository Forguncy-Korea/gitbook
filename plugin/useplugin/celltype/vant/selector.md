# 선택기

현대적인 UI를 가진 포커스 설정 명령의 선택기(콤보박스)를 사용할 수 있습니다.

내장 드롭다운/콤보상자와 비교하면 아래와 같은 이점과 제약사항이 있습니다.&#x20;

### 이점

1. 현대적인 UI 디자인

### 제약사항&#x20;

1. 스타일 템플릿을 지원하지 않음
2. Excel 형식을 지원하지 않습니다.
3. 목록 보기에 셀 유형 추가를 지원하지 않음
4. 검색을 지원하지 않음 <br>



### 빌더화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (966).png" alt=""><figcaption></figcaption></figure>



### 실행화면 (런타임)

<figure><img src="../../../../.gitbook/assets/image (983).png" alt=""><figcaption></figcaption></figure>



### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (975).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="284">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>명령 편집</td><td>값이 변경될 때 실행할 명령 구성</td></tr><tr><td>데이터 유효성 검사</td><td>셀의 구성 데이터 유효성 검사, 업데이트 명령 실행 또는 요청 서버 명령 실행 시에만 유효성 검사</td></tr><tr><td>UI 권한</td><td>현재 사용자의 역할에 따라 표시/편집 가능/활성화 권한</td></tr><tr><td>기본값</td><td>기본값</td></tr><tr><td>바인딩 사용</td><td>항목이 데이터베이스에서 바인딩되는지 여부를 나타냅니다 <br>. 항목이 데이터베이스에서 온 경우 선택기는 중복 항목을 자동으로 제거합니다. <br></td></tr><tr><td>항목 구성 </td><td>디자인 타임에 바인딩 해제 항목 구성</td></tr><tr><td>바인딩 항목 구성 </td><td>구성 바인딩 항목. 구성 값/레이블 열, 필터, 정렬, 상단/오프셋 및 캐시 허용</td></tr><tr><td>자리 표시자</td><td>텍스트 상자 자리 표시자</td></tr><tr><td>접두사 아이콘</td><td><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197565/image2022-3-28_13-37-55.png?version=1&#x26;modificationDate=1648445876463&#x26;cacheVersion=1&#x26;api=v2&#x26;width=215&#x26;height=60" alt=""></td></tr><tr><td>접미사 아이콘</td><td><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197565/image2022-3-28_13-38-18.png?version=1&#x26;modificationDate=1648445899333&#x26;cacheVersion=1&#x26;api=v2&#x26;width=189&#x26;height=68" alt=""></td></tr><tr><td>내부 테두리 표시</td><td><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197565/image2022-3-28_13-39-5.png?version=1&#x26;modificationDate=1648445945593&#x26;cacheVersion=1&#x26;api=v2&#x26;width=209&#x26;height=66" alt=""></td></tr><tr><td>지우기 아이콘 활성화</td><td><p>선택한 항목이 비어 있지 않을 때 접미사 지우기 아이콘을 표시할지 여부를 결정합니다.</p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197565/image2022-3-28_13-50-54.png?version=1&#x26;modificationDate=1648446655073&#x26;cacheVersion=1&#x26;api=v2&#x26;width=208&#x26;height=64" alt=""></p></td></tr><tr><td>읽기 전용</td><td>읽기 전용<br></td></tr><tr><td>비활성화 </td><td>비활성화 </td></tr><tr><td>팝업 구성</td><td><p>도구 모음 표시: 팝업에 상단 표시줄 표시 여부를 결정합니다.</p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197565/image2022-3-28_13-52-13.png?version=1&#x26;modificationDate=1648446733743&#x26;cacheVersion=1&#x26;api=v2&#x26;width=281&#x26;height=250" alt=""></p><p>위쪽 제목</p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197565/image2022-3-28_13-54-3.png?version=1&#x26;modificationDate=1648446843307&#x26;cacheVersion=1&#x26;api=v2&#x26;width=293&#x26;height=250" alt=""></p><p>확인 버튼 텍스트 </p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197565/image2022-3-28_13-54-35.png?version=1&#x26;modificationDate=1648446875893&#x26;cacheVersion=1&#x26;api=v2&#x26;width=287&#x26;height=250" alt=""></p><p>취소 버튼 텍스트</p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197565/image2022-3-28_13-55-9.png?version=1&#x26;modificationDate=1648446909897&#x26;cacheVersion=1&#x26;api=v2&#x26;width=291&#x26;height=250" alt=""></p><p>표시 가능한 항목 개수: 보이는 열의 개수</p><p>항목 높이(픽셀): 항목 높이</p><p>살짝 밀기 기간 : 모멘텀 애니메이션의 지속 시간, 단위 ms</p></td></tr></tbody></table>

## &#x20;관련 명령 빠른 생성  <a href="#vantselector-availableoperations" id="vantselector-availableoperations"></a>

<table><thead><tr><th width="311">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>팝업 표시</td><td>옵션 선택기 열기</td></tr><tr><td>문자열 배열로 데이터 소스 설정</td><td>동적 JSON 문자열 배열을 셀의 데이터 소스로 사용하여 json 형식 예는 다음과 같습니다.<br>[<br>    "Banana",<br>    "Apple",<br>    "Pear"<br>]<br>일반적으로 데이터 소스는 HTTP 요청 명령을 통해 웹 서비스에서 얻을 수 있습니다. 또는 서버 측 명령을 통해 얻을 수 있습니다.</td></tr><tr><td>개체 배열로 데이터 소스 설정</td><td>동적 JSON 객체를 셀의 데이터 소스로 사용하는 JSON 형식의 예는 다음과 같습니다.<br>[<br>    {"value": 1, "label": "Banana"},<br>    {"value": 2, "label": "Apple "},<br>    {"value": 3, "label": "Pear"}<br>]<br>위의 데이터는 '값 속성'이 값이고 '레이블 속성 이름'이 레이블이라고 가정합니다<br>. 일반적으로 JSON 데이터 소스는 다음에서 얻을 수 있습니다. HTTP 요청 명령을 통해 또는 서버 측 명령에서 웹 서비스</td></tr><tr><td>표시 텍스트 가져오기</td><td>현재 표시 텍스트를 가져와 새 변수에 저장합니다. 매개변수: 변수 이름, 기본값은 "Display_Text"입니다.</td></tr></tbody></table>
