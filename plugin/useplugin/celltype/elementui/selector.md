# 항목선택기

기본으로 제공하는 콤보박스  셀타입 보다 아름다운 디자인을 가진 Element UI의 항목선택기를 사용할 수 있습니다.&#x20;

기본으로 제공하는 콤보박스셀타입과 비교하면 아래와 같은 장점과 제약사항이 있습니다.

### 장점&#x20;

* 현대적인 UI 스타일&#x20;
* 서버 단 검색 지원
* 모바일 페이지에서도 입력 지원
* 바인딩 시 서버단 캐시를 지원&#x20;

### 제약사항

* 리스트뷰에서 사용이 가능하지 않음
* 포커스를 받을 때 모든 텍스트 선택을 지원하지 않음
* 스타일 템플릿을 지원하지 않음
* Excel을 지원하지 않음
* 항목선택기에서 여러 열은 지원하지 않음
* 드롭다운 버튼표시를 지원하지 않음&#x20;
* 사용자 지정 드롭다운 너비를 지원하지 않음&#x20;
* "최대 드롭다운 항목 수"를 지원하지 않음&#x20;

<figure><img src="../../../../.gitbook/assets/image (1305).png" alt=""><figcaption></figcaption></figure>



### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (1273).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="283">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>명령 편집</td><td>값이 변경될 때 실행할 명령 구성</td></tr><tr><td>데이터 유효성 검증</td><td>셀의 구성 데이터 유효성 검사, 업데이트 명령 실행 또는 요청 서버 명령 실행 시에만 유효성 검사</td></tr><tr><td>UI 권한 편집 </td><td>현재 사용자의 역할에 따라 권한 표시/활성화</td></tr><tr><td>기본값</td><td>기본값</td></tr><tr><td>데이터연동 </td><td>항목이 데이터베이스에서 바인딩되는지 여부를 나타냅니다 <br>. 항목이 데이터베이스에서 온 경우 선택기는 중복 항목을 자동으로 제거합니다. </td></tr><tr><td>항목구성 </td><td>디자인 타임에 바인딩 해제 항목 구성</td></tr><tr><td>구성 바인딩 항목</td><td>구성 바인딩 항목. 구성 값/레이블 열, 필터, 정렬, 상단/오프셋 및 캐시 허용</td></tr><tr><td>빈 항목 추가</td><td>UseBinding이 true인 경우에만 사용 가능</td></tr><tr><td>빈항목 텍스트 </td><td>값이 없는 경우 표시할 내용을 설정</td></tr><tr><td>다중 선택 모드 </td><td>여러 항목 선택 허용 여부<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197212/image2022-2-16_15-4-26.png?version=1&#x26;modificationDate=1644995067090&#x26;cacheVersion=1&#x26;api=v2&#x26;width=220&#x26;height=250" alt=""></td></tr><tr><td>다중 선택 모드 시 숫자 표시 </td><td>다중이 참인 경우에만 사용 가능<br>참<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197212/image2022-2-16_15-5-31.png?version=1&#x26;modificationDate=1644995132187&#x26;cacheVersion=1&#x26;api=v2&#x26;width=227&#x26;height=250" alt=""><br>거짓<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197212/image2022-2-16_15-5-11.png?version=1&#x26;modificationDate=1644995111847&#x26;cacheVersion=1&#x26;api=v2&#x26;width=220&#x26;height=250" alt=""></td></tr><tr><td>최대 다중 선택 수 </td><td>다중이 참인 경우에만 사용할 수 있으며 선택할 수 있는 최대 항목 수를 나타냅니다.</td></tr><tr><td>항목 검색 가능 </td><td>사용자가 입력 상자에 키워드를 입력하여 항목을 검색할 수 있는지 여부를 나타냅니다.</td></tr><tr><td>입력 검색어 유지 </td><td>다중이 참인 경우에만 사용할 수 있습니다. 사용자가 항목을 선택할 때 명확한 키워드인지 여부를 나타냅니다.</td></tr><tr><td>직접 입력 생성 허용 </td><td>사용자가 드롭다운 항목에 없는 값을 입력할 수 있음을 나타냅니다.</td></tr><tr><td>서버내 데이터 연동 검색 설정 </td><td>바인딩 모드에서만 사용할 수 있습니다. 필터 인 서버 옵션을 사용하여 세부 구성을 설정합니다.<br><img src="../../../../.gitbook/assets/image (1325).png" alt=""></td></tr><tr><td>일치하는 텍스트 없음</td><td>검색 키워드로 항목을 찾지 못한 텍스트입니다.</td></tr><tr><td>선택 후 지우기 버튼 표시</td><td>텍스트가 비어 있지 않고 셀 위로 마우스를 가져가면 지우기 아이콘 표시<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197212/image2022-2-16_15-29-12.png?version=1&#x26;modificationDate=1644996552570&#x26;cacheVersion=1&#x26;api=v2&#x26;width=249&#x26;height=67" alt=""></td></tr><tr><td>비활성화</td><td><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197212/image2022-2-16_15-30-35.png?version=1&#x26;modificationDate=1644996635433&#x26;cacheVersion=1&#x26;api=v2&#x26;width=240&#x26;height=57" alt=""></td></tr></tbody></table>



### 관련 명령 빠른 생성&#x20;

| 명령                 | 설명                                                                                                                                                                                                                                                                                                                 |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 데이터 소스 설정 (문자열 배열) | <p>동적 JSON 문자열 배열을 셀의 데이터 소스로 사용하여 json 형식 예는 다음과 같습니다.<br>[<br>    "Banana",<br>    "Apple",<br>    "Pear"<br>]<br>일반적으로 데이터 소스는 HTTP 요청 명령을 통해 웹 서비스에서 얻을 수 있습니다. 또는 서버 측 명령을 통해 얻을 수 있습니다.</p>                                                                                                                  |
| 데이터 소스 설정 (객체 배열)  | <p>동적 JSON 객체를 셀의 데이터 소스로 사용하는 JSON 형식의 예는 다음과 같습니다.<br>[<br>    {"value": 1, "label": "Banana"},<br>    {"value": 2, "label": "Apple "},<br>    {"value": 3, "label": "Pear"}<br>]<br>위의 데이터는 '값 속성'이 값이고 '레이블 속성 이름'이 레이블이라고 가정합니다<br>. 일반적으로 JSON 데이터 소스는 다음에서 얻을 수 있습니다. HTTP 요청 명령을 통해 또는 서버 측 명령에서 웹 서비스</p> |
| 커서 이동              | 입력 상자에 커서 맞추기                                                                                                                                                                                                                                                                                                      |
| 연동 데이터 새로고침        | <p>바인딩 모드에서만 사용 가능<br> 바인딩이 변경되었지만 바인딩 항목이 데이터를 자동으로 다시 로드할 수 없는 경우 이 작업을 사용하면 바인딩 항목을 강제로 다시 로드할 수 있습니다.</p>                                                                                                                                                                                                      |
| 표시 텍스트 가져오기        | 표시된 텍스트를 가져옵니다.                                                                                                                                                                                                                                                                                                    |
