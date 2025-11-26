# 페이지 매김

페이지 매김 셀타입은  리스트뷰의 페이지를 넘길 수 있습니다.

셀값은 현재 페이지의 번호를 의미합니다.&#x20;

내장된 페이지 탐색  셀타입과  비교할 때 이 셀 유형은 다음과 같은 이점이 있습니다.

1. 현대적인 UI 디자인
2. 사용자가 런타임에서 한 페이지 행 수를 변경할 수 있습니다.

<figure><img src="../../../../.gitbook/assets/image (1671).png" alt=""><figcaption></figcaption></figure>



### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (1967).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="258">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>페이지 변경 명령</td><td>페이지 인덱스 또는 페이지 크기가 UI에 의해 변경될 때 실행할 명령을 구성합니다.</td></tr><tr><td>리스트뷰   선택</td><td>페이지 매김의 대상 리스트뷰를 선택하십시오.<br>페이지가 여러 개인 경우 동일한 리스트뷰를 선택합니다. 페이지 수, 페이지 색인과 같은 설정은 동기화됩니다.</td></tr><tr><td>표시 모드</td><td><p>멀티 </p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931196589/image2022-5-6_15-41-1.png?version=1&#x26;modificationDate=1651822861487&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>심플 </p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931196589/image2022-5-6_15-41-43.png?version=1&#x26;modificationDate=1651822903303&#x26;cacheVersion=1&#x26;api=v2" alt=""></p></td></tr><tr><td>표시할 페이지 크기의  개수</td><td>표시할 페이지 크기 수</td></tr><tr><td>페이지 당 항목 수 </td><td>페이지당 항목 번호</td></tr><tr><td>이전 텍스트</td><td>이전 버튼의 텍스트 사용자 지정</td></tr><tr><td>다음 텍스트</td><td>다음 버튼의 텍스트 사용자 지정</td></tr><tr><td>줄임표 강제  지정 </td><td><p>버튼 수가 초과되면 줄임표를 표시합니다 . 페이지 크기를 표시합니다.</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931196589/image2022-5-6_15-47-12.png?version=1&#x26;modificationDate=1651823232947&#x26;cacheVersion=1&#x26;api=v2" alt=""></p></td></tr></tbody></table>



### 관련 명령 빠른 생성&#x20;

<table><thead><tr><th width="271">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>페이지당 항목 설정</td><td>페이지당 항목 설정</td></tr><tr><td>현재 페이지 설정</td><td>현재 페이지 설정</td></tr><tr><td>총 개수 설정</td><td>listview Name이 null인 경우에만 사용 가능</td></tr><tr><td>명령 실행 </td><td>페이지 변경 명령 ​​즉시 실행</td></tr></tbody></table>
