# ConvertOADateToDate 메서드

### 메서드&#x20;

Forguncy.ConvertOADateToDate(oaDate)

### 설명&#x20;

이 메서드를 사용하여 OADATE에서 DateTime으로 변환합니다.

### 매개변수&#x20;

| 매개변수   | 형식     | 설명     |
| ------ | ------ | ------ |
| oaDate | number | OADate |

### 반환값&#x20;

Date,  OADate에서 변환된 날짜입니다.

### 예제&#x20;

```javascript
//OADate 가져오기
var oaDate = 40000;
//OADate를 DateTime으로 변환
var date = Forguncy.ConvertOADateToDate(oaDate);
//변환된 날짜를 보여주는 경고 상자 팝업
alert(date);
```

### 사용 예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364529/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092717000\&api=v2) 페이지에서 셀 범위를 선택하고 셀 유형을 단추로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (1874).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364529/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092716000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 OADate 변환 버튼을 클릭하면 변환된 날짜를 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (1635).png" alt=""><figcaption></figcaption></figure>
