# 아바타

내장이미지를 아바타 셀타입을 이용하여 사용할 수 있습니다.&#x20;

이미지 셀타입과 비교하면 아래와 같은 장점과 제약사항이 있습니다.

### 장점&#x20;

* 포건시 사용자의 아바타 표시 지원&#x20;
* 아바타를 찾을 수 없는 경우 사용자 이름 표시 지원&#x20;



### 제약사항

* 리스트뷰에서 사용이 가능하지 않음
* 스타일 템플릿을 지원하지 않음



### 빌더화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (486).png" alt=""><figcaption></figcaption></figure>



### 실행 화면 (런타임)

<figure><img src="../../../../.gitbook/assets/image (2041).png" alt=""><figcaption></figcaption></figure>



### 셀 속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (488).png" alt=""><figcaption></figcaption></figure>

| 이름         | 설명                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 클릭 명령      | 셀을 클릭할 때 실행할 명령 구성                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| 기본 아바타     | <p>이미지 값이 없으면 아바타 셀에 아이콘이 표시되거나 사용자 이름이 표시됩니다.<br>아이콘 설정:<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196131/image2022-2-17_18-4-19.png?version=1&#x26;modificationDate=1645092259120&#x26;cacheVersion=1&#x26;api=v2&#x26;width=76&#x26;height=70" alt=""></p><p>아이콘을 설정하지 않음:<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196131/image2022-2-17_18-4-48.png?version=1&#x26;modificationDate=1645092288823&#x26;cacheVersion=1&#x26;api=v2&#x26;width=75&#x26;height=73" alt=""></p> |
| 아바타 모양     | <p>정사각형<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196131/image2022-2-17_18-4-19.png?version=1&#x26;modificationDate=1645092259120&#x26;cacheVersion=1&#x26;api=v2&#x26;width=76&#x26;height=70" alt=""><br>원<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196131/image2022-2-17_18-5-44.png?version=1&#x26;modificationDate=1645092344597&#x26;cacheVersion=1&#x26;api=v2&#x26;width=81&#x26;height=75" alt=""></p>                                                                  |
| 맞추기        | <ul><li>채우기</li><li>포함</li><li>커버 </li><li>원본크기 </li><li>축소</li></ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| 시스템 아바타 표시 | 체크하면 아바타 셀유형은 시스템 기본 사용자 이름을 셀 값에 표시합니다. 현재 사용자의 이름이 "홍길동"이라면 "홍길동"의 아바타를 표시하려 시도하지만, 이 아바타가 설정되지 않은 경우 셀에 사용자 이름을 대신 표시합니다. 사용자 이름을 가져오려는 경우 "UserInfoView" 또는 "%CurrentUser%" 키워드를 사용하세요.                                                                                                                                                                                                                                                                                                                                                       |

<br>
