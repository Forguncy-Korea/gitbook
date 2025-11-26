# 숫자

모바일 화면에서 숫자를 입력할 수 있는 셀타입니다.

내장 숫자  셀타입과 비교하면 아래와 같은 이점과 제약사항이 있습니다.&#x20;

### 이점

1. 현대적인 UI 디자인
2. 입력 시 최대 길이 지원

### 제약사항

1. 목록 보기에 셀 유형 추가를 지원하지 않음
2. 스타일 템플릿을 지원하지 않음
3. 1000 구분 기호를 지원하지 않음
4. Excel 형식을 지원하지 않음



### 빌더 화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (996).png" alt=""><figcaption></figcaption></figure>



### 실행 화면 (런타임)&#x20;

<figure><img src="../../../../.gitbook/assets/image (934).png" alt=""><figcaption></figcaption></figure>



### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (959).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="307">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>명령 편집</td><td>값이 변경될 때 실행할 명령 구성</td></tr><tr><td>데이터 유효성 검사</td><td>셀의 구성 데이터 유효성 검사, 업데이트 명령 실행 또는 요청 서버 명령 실행 시에만 유효성 검사</td></tr><tr><td>UI 권한</td><td>현재 사용자의 역할에 따라 권한 표시/활성화</td></tr><tr><td>기본값</td><td>기본값</td></tr><tr><td>최대 길이</td><td>입력 숫자의 최대 길이</td></tr><tr><td>자리 표시자</td><td>자리 표시자</td></tr><tr><td>접두사 아이콘</td><td>텍스트 상자의 접두사 아이콘</td></tr><tr><td>접미사 아이콘 </td><td>텍스트 상자의 접미사 아이콘</td></tr><tr><td>내부 테두리 표시</td><td>하단 테두리 표시 여부 결정</td></tr><tr><td>지우기 아이콘 활성화</td><td>텍스트 상자의 모든 콘텐츠를 지울 수 있는 접미사 지우기 아이콘 표시 여부 결정</td></tr><tr><td>숫자로 변환</td><td>입력 텍스트를 숫자로 변환할지 여부 결정</td></tr><tr><td>읽기 전용</td><td>수정이  불가능하고 읽을 수만 있음 <br></td></tr><tr><td>비활성화 </td><td>비활성화 <br></td></tr><tr><td>숫자 키패드 설정</td><td><p>제목: 키패드 제목</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197517/image2022-3-28_11-24-21.png?version=1&#x26;modificationDate=1648437862080&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>닫기 버튼 텍스트</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197517/image2022-3-28_11-25-40.png?version=1&#x26;modificationDate=1648437940333&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>삭제 버튼 텍스트 </p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197517/image2022-3-28_11-26-33.png?version=1&#x26;modificationDate=1648437993507&#x26;cacheVersion=1&#x26;api=v2&#x26;width=326&#x26;height=221" alt=""></p><p>추가 키 텍스트</p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197517/image2022-3-28_11-27-52.png?version=1&#x26;modificationDate=1648438072990&#x26;cacheVersion=1&#x26;api=v2&#x26;width=325&#x26;height=224" alt=""></p><p>오른쪽 열 표시: 오른쪽 열이 표시되면 두 개의 추가 키를 구성할 수 있습니다.</p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197517/image2022-3-28_11-32-58.png?version=1&#x26;modificationDate=1648438378823&#x26;cacheVersion=1&#x26;api=v2&#x26;width=496&#x26;height=250" alt=""></p><p>외부 클릭 시 숨기기: 이 옵션을 선택하면 외부를 클릭할 때 키패드가 숨겨집니다.</p><p>임의의 키 순서: 체크하면 키 순서가 랜덤이 됩니다.</p></td></tr></tbody></table>



### 관련 명령 빠른 생성&#x20;

| 이름    | 설명        |
| ----- | --------- |
| 팝업 표시 | 숫자 키패드 표시 |
