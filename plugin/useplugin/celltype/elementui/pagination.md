# 게시판 형태 페이지

기본 제공되는 페이지 탐색과 비교 하였을 때 Element UI의 게시판 형태 페이지 셀타입은 아래와 같은 이점이 있습니다.&#x20;

1. 현대적인 UI 디자인
2. 유연한 레이아웃 설정&#x20;
3. 총 항목 수 표시 허용
4. 사용자가 런타임에서 한 페이지 행 수를 변경할 수 있습니다.
5. 한 페이지만 있는 경우 자동 숨기기



### 빌더 화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (976).png" alt=""><figcaption></figcaption></figure>

### 실행화면 (런타임)

<figure><img src="../../../../.gitbook/assets/image (967).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (1000).png" alt=""><figcaption></figcaption></figure>

| 이름              | 설명                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 페이징 변경 시 명령 실행  | 페이지 인덱스 또는 페이지 크기가 UI에 의해 변경될 때 실행할 명령을 구성합니다.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| 리스트뷰 선택         | <p>페이지 매김의 대상 리스트뷰를 선택하십시오.<br>페이지가 여러 개인 경우 동일한 목록 보기를 선택합니다. 페이지 수, 페이지 색인과 같은 설정은 동기화됩니다.</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 한 페이지에 표시할 항목 수 | 한 페이지의 레코드 수입니다.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 하단 페이지 링크 수     | <p>최대 페이저 인덱스가 페이지 매김에 표시됨을 나타냅니다. 유효성 검사 값은 5-21입니다.<br>예시 값 5<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_16-50-51.png?version=1&#x26;modificationDate=1643446251670&#x26;cacheVersion=1&#x26;api=v2&#x26;width=573&#x26;height=62" alt=""></p><p>예제 값 13<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_16-51-43.png?version=1&#x26;modificationDate=1643446303947&#x26;cacheVersion=1&#x26;api=v2&#x26;width=873&#x26;height=45" alt=""></p>    |
| 주요 표시 항목 구성     | <p>Prev,Pager,Next,Jumper,→,Total, Sizes 지원, 사용자는 요소 레이아웃의 순서를 변경할 수 있습니다. 사용자는 일부 요소도 추가/제거할 수 있습니다.</p><p><img src="../../../../.gitbook/assets/image (1001).png" alt=""><br><br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-0-43.png?version=1&#x26;modificationDate=1643446843843&#x26;cacheVersion=1&#x26;api=v2&#x26;width=841&#x26;height=191" alt=""><br></p>                                                                                                                                |
| 이전 페이지 이동 문구    | <p>이전 버튼의 텍스트 사용자 지정<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-36-24.png?version=1&#x26;modificationDate=1643448984503&#x26;cacheVersion=1&#x26;api=v2&#x26;width=388&#x26;height=41" alt=""></p>                                                                                                                                                                                                                                                                                               |
| 다음 페이지 이동 문구    | <p>다음 버튼의 텍스트 사용자 지정<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-36-28.png?version=1&#x26;modificationDate=1643448988643&#x26;cacheVersion=1&#x26;api=v2&#x26;width=388&#x26;height=41" alt=""></p>                                                                                                                                                                                                                                                                                               |
| 작게 보이기          | <p>페이지 매김 크기<br>보통:<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-37-28.png?version=1&#x26;modificationDate=1643449048450&#x26;cacheVersion=1&#x26;api=v2&#x26;width=723&#x26;height=36" alt=""></p><p>작은:<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-37-40.png?version=1&#x26;modificationDate=1643449060097&#x26;cacheVersion=1&#x26;api=v2&#x26;width=717&#x26;height=34" alt=""></p>                                                    |
| 배경색 표시          | <p>배경 = 거짓(기본값)<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-38-53.png?version=1&#x26;modificationDate=1643449133313&#x26;cacheVersion=1&#x26;api=v2&#x26;width=744&#x26;height=49" alt=""><br>배경 = 참<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-39-4.png?version=1&#x26;modificationDate=1643449144177&#x26;cacheVersion=1&#x26;api=v2&#x26;width=738&#x26;height=51" alt=""></p>                                                         |
| 1페이지만 있을 경우 숨김  | 한 페이지만 있는 경우 셀 유형 숨기기                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| 비활성화            | <p>비활성화 = false(기본값)<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-40-17.png?version=1&#x26;modificationDate=1643449217217&#x26;cacheVersion=1&#x26;api=v2&#x26;width=758&#x26;height=37" alt=""></p><p>비활성화됨 = 참 </p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-40-31.png?version=1&#x26;modificationDate=1643449231390&#x26;cacheVersion=1&#x26;api=v2&#x26;width=737&#x26;height=45" alt=""></p>                                         |
| 페이지 크기          | <p>이 옵션은 레이아웃에 "크기" 항목이 포함된 경우에만 사용할 수 있습니다. 페이지의 드롭다운 항목 표시<br>디자인 타임<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-42-23.png?version=1&#x26;modificationDate=1643449343420&#x26;cacheVersion=1&#x26;api=v2&#x26;width=301&#x26;height=250" alt=""><br>실행 시간<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196634/image2022-1-29_17-42-6.png?version=1&#x26;modificationDate=1643449326900&#x26;cacheVersion=1&#x26;api=v2&#x26;width=695&#x26;height=250" alt=""></p> |

### &#x20;관련 명령 빠른 생성&#x20;

| 이름                 | 설명                           |
| ------------------ | ---------------------------- |
| 한 페이지에 표시할 항목 수 설정 | 한 페이지에 표시할 항목 수 설정할 수 있음     |
| 설정한 페이지로 이동하기      | <p>설정한 페이지로 이동하게  설정<br></p> |
| 직접 입력한 페이지로 이동     | 직접 입력한 페이지로 이동하게 설정          |
