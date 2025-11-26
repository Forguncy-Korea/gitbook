# 숫자표시상자

기본으로 제공하는 숫자형식  셀타입 보다 아름다운 디자인을 가진 Element UI의 숫자표시상자를 사용할 수 있습니다.&#x20;

기본으로 제공하는 숫자형식셀타입과 비교하면 아래와 같은 장점과 제약사항이 있습니다.

### 장점&#x20;

* 현대적인 UI 스타일&#x20;
* 입력 시 최대, 최소값 지원

### 제약사항

* 리스트뷰에서 사용이 가능하지 않음
* 포커스를 받을 때 모든 텍스트 선택을 지원하지 않음
* 스타일 템플릿을 지원하지 않음
* Excel을 지원하지 않음
* 1000구분 기호를 지원하지 않음&#x20;

### 사용방법&#x20;

셀영역을 지정한 후, 상단 셀 유형에서 엘리먼트 UI에서 "숫자표시상자"를 선택합니다.

<figure><img src="../../../../.gitbook/assets/image (1317).png" alt=""><figcaption></figcaption></figure>

### 속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (1694).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="324">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>명령 편집</td><td>값이 변경될 때 실행할 명령 구성</td></tr><tr><td>데이터 유효성 검사</td><td>셀의 구성 데이터 유효성 검사, 업데이트 명령 실행 또는 요청 서버 명령 실행 시에만 유효성 검사</td></tr><tr><td>UI 권한 편집 </td><td>현재 사용자의 역할에 따라 권한 표시/활성화</td></tr><tr><td>기본값</td><td>기본값<br></td></tr><tr><td>최소값 </td><td>입력 가능한 최소값</td></tr><tr><td>최대값 </td><td>입력 가능한 최대값</td></tr><tr><td>증분크기설정 </td><td>실행 시(런타임에서) +, -버튼 클릭 시의 증분 단위</td></tr><tr><td>증분범위와 직접입력 비허용</td><td>체크 시 Step의 정수배가 아닌 값 입력 지원 안함</td></tr><tr><td>소수점 표시 자릿수</td><td>소수 자릿수</td></tr><tr><td>자리 표시자</td><td>텍스트가 비어 있을 때만 표시<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197263/image2022-2-16_13-57-47.png?version=1&#x26;modificationDate=1644991067247&#x26;cacheVersion=1&#x26;api=v2&#x26;width=237&#x26;height=57" alt=""></td></tr><tr><td>증분버튼표시</td><td>컨트롤 표시 또는<br>True 가 아님을 나타냅니다.<br><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197263/image2022-2-16_13-52-48.png?version=1&#x26;modificationDate=1644990768393&#x26;cacheVersion=1&#x26;api=v2" alt=""><br>거짓<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197263/image2022-2-16_13-59-2.png?version=1&#x26;modificationDate=1644991142990&#x26;cacheVersion=1&#x26;api=v2&#x26;width=246&#x26;height=54" alt=""></td></tr><tr><td>증분버튼을 오른쪽에 표시</td><td>컨트롤 표시를 스핀 버튼으로 표시하거나<br>True 가 아님<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197263/image2022-2-16_14-0-45.png?version=1&#x26;modificationDate=1644991245297&#x26;cacheVersion=1&#x26;api=v2&#x26;width=242&#x26;height=55" alt=""><br>거짓<br><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931197263/image2022-2-16_13-52-48.png?version=1&#x26;modificationDate=1644990768393&#x26;cacheVersion=1&#x26;api=v2" alt=""></td></tr><tr><td>비활성화</td><td><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197263/image2022-2-16_14-26-7.png?version=1&#x26;modificationDate=1644992768083&#x26;cacheVersion=1&#x26;api=v2&#x26;width=263&#x26;height=60" alt=""></td></tr></tbody></table>



### 관련 명령  빠른 생성&#x20;

| 이름     | 설명            | 매개변수      |
| ------ | ------------- | --------- |
| 최소값 설정 | 최소값 설정        | 최소값       |
| 최대값 설정 | 최대값 설정        | 최대값       |
| 증분 설정  | 증분 크기 설정      | 증분 크기 설정  |
| 커서이동   | 대상 셀로   커서이동  | -         |
