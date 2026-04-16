# ConvertDateToOADate 메서드

### 메서드

Forguncy.ConvertDateToOADate(date)

### 설명&#x20;

이 메서드를 사용하여 DateTime을 OADate로 변환 합니다.

### 매개 변수



| 매개변수  | 형식   | 설명  |
| ----- | ---- | --- |
| date  | Date | 날짜  |

### 반환값&#x20;

number, 날짜에서 OADate로 변환합니다.



### 예제&#x20;

```
//날짜 가져오기 
var date = new Date();
//DateTime을 OADate로 변환
var oaDate = Forguncy.ConvertDateToOADate(date);
// 경고 상자 팝업, OADate 표시
alert(oaDate);
```

### 사용 예제&#x20;

1. 페이지에서 셀 범위를 선택하고 셀 유형을 단추로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (898).png" alt=""><figcaption></figcaption></figure>

2. 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 날짜 변환 버튼을 클릭하면 변환된 OADate를 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (1055).png" alt=""><figcaption></figcaption></figure>

<br>
