# 날짜/시간 선택기

포커스설정의 날짜/시간 선택기를 이용하여 현대적인 UI 디자인을 모바일페이지에서 사용할 수 있습니다.

내장 DateCellType 및 TimeCellType과 비교하면 아래와 같은 이점과 제약사항이 있습니다.&#x20;

### 이점

1. 현대적인 UI 디자인
2. 지원 접두사 아이콘
3. 지원 접미사 아이콘
4. 지우기 아이콘 지원
5. 결합된 DateCellType 및 TimeCellType

### 제약사항

1. 목록 보기에 셀 유형 추가를 지원하지 않음
2. 포커스를 받을 때 모든 텍스트 선택을 지원하지 않음
3. 스타일 템플릿을 지원하지 않음
4. Excel 형식을 지원하지 않음&#x20;



### 빌더화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (2203).png" alt=""><figcaption></figcaption></figure>

### 실행화면 (런타임)

<figure><img src="../../../../.gitbook/assets/image (1008).png" alt=""><figcaption></figcaption></figure>

### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (981).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="301">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>명령 편집</td><td>값이 변경될 때 실행할 명령 구성</td></tr><tr><td>데이터 유효성 검사</td><td>셀의 구성 데이터 유효성 검사, 업데이트 명령 실행 또는 요청 서버 명령 실행 시에만 유효성 검사</td></tr><tr><td>UI 권한</td><td>현재 사용자의 역할에 따라 표시/편집 가능/활성화 권한</td></tr><tr><td>기본값</td><td>기본값</td></tr><tr><td>유형 선택</td><td><p>날짜 : yyyy MM dd</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-38-7.png?version=1&#x26;modificationDate=1648449487893&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>년-월 : yyyy MM</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-38-58.png?version=1&#x26;modificationDate=1648449539153&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>월-일 : MM dd</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-39-34.png?version=1&#x26;modificationDate=1648449574980&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>날짜-시간 : yyyy MM dd HH</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-40-33.png?version=1&#x26;modificationDate=1648449633873&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>날짜 시간 : yyyy MM dd HH mm</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-41-17.png?version=1&#x26;modificationDate=1648449677843&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>시간 : HH mm</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-42-5.png?version=1&#x26;modificationDate=1648449725527&#x26;cacheVersion=1&#x26;api=v2" alt=""></p></td></tr><tr><td>최소 날짜</td><td>최소 날짜</td></tr><tr><td>최대 날짜</td><td>최대 날짜</td></tr><tr><td>최소 시간</td><td> 유형 의 최소 시간<code>time</code> </td></tr><tr><td>최대 시간</td><td> 유형 의 최대 시간<code>time</code> </td></tr><tr><td>최소 분</td><td> 유형 의 최소 분<code>time</code> </td></tr><tr><td>최대 분</td><td> 유형 의 최대 분<code>time</code> </td></tr><tr><td>자리 표시자</td><td>자리 표시자</td></tr><tr><td>접두사 아이콘</td><td><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197626/image2022-3-28_14-49-46.png?version=1&#x26;modificationDate=1648450186140&#x26;cacheVersion=1&#x26;api=v2&#x26;width=250&#x26;height=72" alt=""></td></tr><tr><td>접미사 아이콘</td><td><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197626/image2022-3-28_14-50-12.png?version=1&#x26;modificationDate=1648450212700&#x26;cacheVersion=1&#x26;api=v2&#x26;width=252&#x26;height=58" alt=""></td></tr><tr><td>내부 테두리 표시</td><td><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197626/image2022-3-28_14-51-39.png?version=1&#x26;modificationDate=1648450299533&#x26;cacheVersion=1&#x26;api=v2&#x26;width=300&#x26;height=70" alt=""></td></tr><tr><td>지우기 아이콘 활성화</td><td>접미사 지우기 아이콘 표시 여부</td></tr><tr><td>읽기 전용</td><td><br></td></tr><tr><td>비활성화</td><td><br></td></tr><tr><td>팝업 구성</td><td><p>도구 모음 표시: 팝업에 상단 표시줄 표시 여부를 결정합니다.</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-54-11.png?version=1&#x26;modificationDate=1648450451710&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>위쪽 제목</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-54-26.png?version=1&#x26;modificationDate=1648450466523&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>확인 버튼 텍스트 </p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-54-50.png?version=1&#x26;modificationDate=1648450490847&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>취소 버튼 텍스트</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197626/image2022-3-28_14-55-6.png?version=1&#x26;modificationDate=1648450506737&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>표시 가능한 항목 개수 : 보이는 열의 개수 </p><p>항목 높이(픽셀): 항목 높이</p><p>살짝 밀기 기간 : 모멘텀 애니메이션의 지속 시간, 단위  ms</p></td></tr></tbody></table>



### 관련 명령 빠른 생성&#x20;

| 이름    | 설명           |
| ----- | ------------ |
| 팝업 표시 | 날짜/시간 선택기 열기 |
