# 입력상자

기본으로 제공하는 텍스트상자보다 아름다운 디자인을 가진 Element UI의 입력상자를 사용할 수 있습니다.&#x20;

기본으로 제공하는 텍스트상자와 비교하면 아래와 같은 장점과 제약사항이 있습니다.

### 장점&#x20;

* 최대길이를 설정하여 사용 가능
* 모든 텍스트를 지우는 기능 제공&#x20;

### 제약사항

* 리스트뷰에서 사용이 가능하지 않음
* 포커스를 받을 때 모든 텍스트 선택을 지원하지 않음
* 스타일 템플릿을 지원하지 않음
* Excel을 지원하지 않음





### 사용방법&#x20;

셀영역을 지정한 후, 상단 셀 유형에서 엘리먼트 UI에서 "입력상자"를 선택합니다.

<figure><img src="../../../../.gitbook/assets/image (1691).png" alt=""><figcaption></figcaption></figure>



### 속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (1308).png" alt=""><figcaption></figcaption></figure>

| 이름          | 설명                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 명령 편집       | 값이 변경될 때 실행할 명령 구성                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| 데이터 유효성 검증  | 셀의 구성 데이터 유효성 검사, 업데이트 명령 실행 또는 요청 서버 명령 실행 시에만 유효성 검사                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| UI 권한 편집    | 현재 사용자의 역할에 따라 표시/편집 가능/활성화 권한                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| 기본값         | 기본값                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| 유형          | <p>한 줄 입력<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-20-17.png?version=1&#x26;modificationDate=1644985217493&#x26;cacheVersion=1&#x26;api=v2&#x26;width=249&#x26;height=61" alt=""><br>비밀번호   형태 표시 <img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-20-52.png?version=1&#x26;modificationDate=1644985253107&#x26;cacheVersion=1&#x26;api=v2&#x26;width=250&#x26;height=58" alt=""><br>여러줄 입력 </p><p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-21-47.png?version=1&#x26;modificationDate=1644985307493&#x26;cacheVersion=1&#x26;api=v2&#x26;width=248&#x26;height=98" alt=""></p> |
| 최대 길이       | 이 옵션은 "단어 제한 표시" 옵션 가시성에 영향을 미칩니다.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| 입력 안내       | <p>유형이 Text 또는 TextArea이고 <strong>MaxLength가</strong> 설정된 경우에만 지원됩니다.<br>텍스트<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-22-45.png?version=1&#x26;modificationDate=1644985365903&#x26;cacheVersion=1&#x26;api=v2&#x26;width=242&#x26;height=53" alt=""></p><p>텍스트 영역<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-21-47.png?version=1&#x26;modificationDate=1644985307493&#x26;cacheVersion=1&#x26;api=v2&#x26;width=248&#x26;height=98" alt=""></p>                                                                                                                                                                              |
| 앞쪽 표시 아이콘   | ![](https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-24-59.png?version=1\&modificationDate=1644985499763\&cacheVersion=1\&api=v2\&width=244\&height=63)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| 뒤쪽 표시 아이콘   | ![](https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-25-43.png?version=1\&modificationDate=1644985543490\&cacheVersion=1\&api=v2\&width=249\&height=58)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| 읽기 전용       | <p><br></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| 비활성화        | ![](https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-27-10.png?version=1\&modificationDate=1644985630673\&cacheVersion=1\&api=v2\&width=246\&height=64)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| 지우기 버튼 표시   | <p>텍스트가 비어 있지 않으면 지우기 아이콘을 표시하고 지우기 아이콘을 클릭하면 텍스트가 지워집니다.<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931197247/image2022-2-16_12-26-13.png?version=2&#x26;modificationDate=1648434788210&#x26;cacheVersion=1&#x26;api=v2&#x26;width=243&#x26;height=61" alt=""></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                |



### 관련 명령 빠른 생성&#x20;

| 이름     | 설명                          |
| ------ | --------------------------- |
| 커서 이동  | 입력 상자에 포커스 맞추기              |
| 텍스트선택  | 입력 상자에 포커스를 맞춘 다음 모든 텍스트 선택 |
