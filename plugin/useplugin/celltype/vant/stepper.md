# 스탭퍼

-, +버튼을 클릭하여 모바일화면에서 숫자를 입력할 수 있습니다. &#x20;

내장 NumberCellType과 비교하면 아래와 같은 이점과 제약사항이 있습니다.&#x20;

### 이점

1. 현대적인 UI 디자인
2. 입력 시 최대/최소값 지원

### 제약사항&#x20;

1. 목록 보기에 셀 유형 추가를 지원하지 않음
2. 포커스를 받을 때 모든 텍스트 선택을 지원하지 않음
3. 스타일 템플릿을 지원하지 않음
4. 1000 구분 기호를 지원하지 않음
5. Excel 형식을 지원하지 않음



### 빌더화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (1006).png" alt=""><figcaption></figcaption></figure>



### 실행화면 (런타임)

<figure><img src="../../../../.gitbook/assets/image (980).png" alt=""><figcaption></figcaption></figure>



### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (1770).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="249">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>명령 편집</td><td>값이 변경될 때 실행할 명령 구성</td></tr><tr><td>데이터 유효성 검사</td><td>셀의 구성 데이터 검증</td></tr><tr><td>UI 권한</td><td>현재 사용자의 역할에 따라 권한 표시/활성화</td></tr><tr><td>기본값</td><td>기본값<br></td></tr><tr><td>최소 </td><td>최소값<br></td></tr><tr><td>최대</td><td>최대값<br></td></tr><tr><td>단계 크기</td><td>단계 크기<br></td></tr><tr><td>10진수길이</td><td>소수점 길이 </td></tr><tr><td>자리 표시자</td><td>텍스트가 비어 있을 때만 표시<br><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931196597/image2022-5-6_16-7-23.png?version=1&#x26;modificationDate=1651824443247&#x26;cacheVersion=1&#x26;api=v2" alt=""></td></tr><tr><td>테마 </td><td><p>직사각형</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931196597/image2022-5-6_16-3-12.png?version=1&#x26;modificationDate=1651824192687&#x26;cacheVersion=1&#x26;api=v2" alt=""></p><p>원</p><p><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931196597/image2022-5-6_16-8-22.png?version=1&#x26;modificationDate=1651824502420&#x26;cacheVersion=1&#x26;api=v2" alt=""></p></td></tr><tr><td>버튼 크기</td><td>버튼 크기   설정<br></td></tr><tr><td>정수만 허용</td><td>UI 입력만 제어</td></tr><tr><td>빈값 허용 </td><td>빈 문자열 입력 허용 여부</td></tr><tr><td>입력 표시</td><td><br>입력 표시</td></tr><tr><td>더하기 버튼 표시</td><td>더하기 버튼 표시</td></tr><tr><td>빼기 버튼 표시</td><td>빼기 버튼 표시</td></tr><tr><td>비활성화 </td><td>비활성화 <br></td></tr><tr><td>입력 비활성화</td><td>입력 비활성화<br></td></tr><tr><td>길게 누르기 허용</td><td>버튼을 길게 누를 때 값을 변경할지 여부</td></tr></tbody></table>



### 관련 명령  빠른 생성&#x20;

| 이름       | 설명                  | 매개변수        |
| -------- | ------------------- | ----------- |
| 최소값 설정   | 최소값 설정              | 최소값         |
| 최대값 설정   | 최대값 설정              | 최대값         |
| 단계 크기 설정 | <p>단계 크기 설정<br></p> | 단계          |
| 초점 설정    | 입력 상자에 초점 맞추기       | <p><br></p> |
