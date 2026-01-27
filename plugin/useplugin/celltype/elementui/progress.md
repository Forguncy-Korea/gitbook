# 진행률

사용자는 진행률 셀타입을 사용하여 진행률을 표시줄에 표시할 수 있습니다.&#x20;

![](<../../../../.gitbook/assets/image (995).png>)

### 셀속성&#x20;

<table><thead><tr><th width="174">이름 </th><th>설명 </th></tr></thead><tbody><tr><td><p>값 변경 시 </p><p>실행할 명령 편집</p></td><td>셀 값이 변경될 때 명령이 실행되도록 구성</td></tr><tr><td>유형</td><td>선, 원 및 대시보드를 포함하는 셀 유형의 디스플레이 유형</td></tr><tr><td>스토크 너비 </td><td>기본값은 6이고 단위는 픽셀입니다.</td></tr><tr><td>상태</td><td>진행 상태를 나타내며 사용 가능한 값은 "없음","성공","경고","오류"입니다<br>. 상태가 없음인 경우에만 진행률 텍스트를 표시할 수 있습니다.</td></tr><tr><td>색상</td><td>진행 색상을 나타냅니다. 상태가 없음일 때만 사용할 수 있습니다.<br>색상을 빨간색으로 설정합니다.</td></tr><tr><td>텍스트 내부</td><td><p>텍스트 위치 표시, "선"에만 사용 가능, 막대 안에 텍스트를 만들 경우 20보다 큰 획 너비 제안<br>텍스트 내부 = false<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196551/image2022-1-30_11-25-29.png?version=1&#x26;modificationDate=1643513129267&#x26;cacheVersion=1&#x26;api=v2&#x26;width=409&#x26;height=54" alt=""></p><p>내부 텍스트 = true<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196551/image2022-1-30_11-25-47.png?version=1&#x26;modificationDate=1643513147977&#x26;cacheVersion=1&#x26;api=v2&#x26;width=425&#x26;height=63" alt=""></p></td></tr><tr><td>텍스트 표시</td><td>텍스트 표시 여부를 나타냅니다. 상태가 없음인 경우에만 사용 가능</td></tr><tr><td>텍스트 수식</td><td>사용자가 진행률 텍스트를 사용자 정의합니다. 기본값은 null이며 백분율 텍스트 표시를 의미합니다. <br>사용자는 ="사용량:" &#x26; A1 &#x26; "Kg of " &#x26; B1 &#x26; "Kg"와 같은 공식을 설정할 수 있습니다.<br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196551/image2022-1-30_11-30-50.png?version=1&#x26;modificationDate=1643513450990&#x26;cacheVersion=1&#x26;api=v2&#x26;width=367&#x26;height=35" alt=""></td></tr></tbody></table>



### 관련 명령 빠른 생성&#x20;

| 배경색 설정 | 색상 설정  |
| ------ | ------ |
| 상태 설정  | 상태 설정  |
