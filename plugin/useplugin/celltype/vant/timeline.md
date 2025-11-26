# 타임라인

타임라인을 시각적으로 표시합니다.

<figure><img src="../../../../.gitbook/assets/image (765).png" alt=""><figcaption></figcaption></figure>

### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (756).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="260">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>변경된 값 편집 명령</td><td>셀 값이 변경될 때 명령이 실행되도록 구성</td></tr><tr><td>기본값</td><td>기본값</td></tr><tr><td>바인딩 사용</td><td>단계 항목이 데이터베이스에서 바인딩되는지 여부를 나타냅니다. </td></tr><tr><td>노드 항목 구성 </td><td>디자인 타임에 바인딩 해제 단계 항목 구성</td></tr><tr><td>바인딩 항목 구성 </td><td>구성 바인딩 단계 항목. 구성 값/제목 열, 필터, 정렬, 상단/오프셋 및 캐시 허용</td></tr><tr><td>활성 아이콘</td><td>활성 아이콘</td></tr><tr><td>비활성 아이콘</td><td>비활성 아이콘</td></tr><tr><td>비활성 색상</td><td>비활성 색상뱇</td></tr><tr><td>배치</td><td><p>타임스탬프의 위치, 하단, 상단으로 설정 가능</p><p>하단 </p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197724/image2022-3-28_17-55-15.png?version=1&#x26;modificationDate=1648461315757&#x26;cacheVersion=1&#x26;api=v2&#x26;width=181&#x26;height=161" alt=""></p><p>상단 </p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197724/image2022-3-28_17-55-32.png?version=1&#x26;modificationDate=1648461332383&#x26;cacheVersion=1&#x26;api=v2&#x26;width=154&#x26;height=147" alt=""></p></td></tr><tr><td>서식 </td><td>타임스탬프 형식 yyyy, yyyy/MM, yyyy/MM/dd, yyyy/MM/dd HH:mm:ss</td></tr></tbody></table>

### 관련 명령 빠른 생성&#x20;

<table><thead><tr><th width="284">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>데이터 소스 설정</td><td>동적 JSON 객체를 셀의 데이터 소스로 사용하는 JSON 형식의 예는 다음과 같습니다.<br>[<br>    {"value": "1", "title": "Activity start", "timestamp": "2018-04-15" },<br>    {"value": "2", "title": "승인됨", "timestamp": "2018-04-13"}, {"value"<br>    : "3", "title": "성공 만들기", "timestamp": "2018-04-11"}<br>]<br>위의 데이터는 '값 속성'이 값이고 '제목 속성'이 콘텐츠이고 '타임스탬프 속성 이름'이 타임스탬프라고 가정합니다. 일반적으로<br>JSON 데이터 소스는 다음과 같습니다. HTTP 요청 명령을 통해 웹 서비스에서 얻은또는 서버 측 명령에서</td></tr><tr><td>활성 아이콘 업데이트</td><td>활성 아이콘 업데이트</td></tr><tr><td>활성 색 업데이트</td><td>활성 색상 업데이트</td></tr></tbody></table>
