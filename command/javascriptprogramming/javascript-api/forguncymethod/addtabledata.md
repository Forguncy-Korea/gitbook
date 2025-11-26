# addTableData 메서드

### 메서드&#x20;

Forguncy.addTableData(tableName, newValue, successCallback, errorCallback)

### 설명&#x20;

이 메서드를 사용하여 지정 된 데이터 테이블에 대한 데이터를 추가 합니다.

### 매개 변수 설명&#x20;

| 매개변수            | 형식                              | 설명                                      |
| --------------- | ------------------------------- | --------------------------------------- |
| tableName       | string                          | 레코드를 추가할 데이터 테이블의 이름입니다.                |
| newValue        | plainObject                     | 테이블의 모든 열을 포함할 필요 없이 행의 열 이름과 값을 추가합니다. |
| successCallback | function( plainObject data )    | 삽입된 행의 값을 포함하는 인수가 있는 함수를 성공적으로 콜백했습니다. |
| errorCallback   | function( string errorMessage ) | 매개 변수에 오류 메시지가 포함된 콜백 함수가 실패했습니다.       |

### 반환값&#x20;

없음

### 예제&#x20;

다음 예제 코드에서는 addTableData 메서드를 사용하여 지정된 데이터 테이블에 데이터를 추가합니다.

```javascript
//지정된 데이터 테이블에 데이터 추가
Forguncy.addTableData("직원테이블",
{
//컬럼 이름과 데이터 지정
이름: "리시",
입사년: "1993/3/1",
부서: "개발 부서"
},
//추가에 성공하면 추가 성공을 알리는 경고 상자가 팝업됩니다.
function (data) {
alert("성공적으로 추가되었습니다.");
},
//추가 실패시 경고창이 뜨면서 실패 정보가 팝업된다.
function (errorMessage) {
alert(errorMessage);
}
);
```

{% hint style="info" %}
\[옵션-> 응용 프로그램 실행]에서 "JavaScript Api를 사용하여 데이터베이스에 접근하여 내용을 변경할 수 없습니다." 선택하면 이 메서드를 사용하여 지정된 데이터 테이블에 데이터를 추가할 때 실패합니다. 이 메서드를 사용 하 여이 메서드를 사용 하 여이 작업을 수행 하기 전에이 옵션을 선택 취소 합니다.

![](<../../../../.gitbook/assets/image (2181).png>)
{% endhint %}

![](https://help.grapecity.com.cn/download/thumbnails/72364571/16.png?version=1\&modificationDate=1648092717000\&api=v2) **사용예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364571/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092717000\&api=v2) 페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 각 열의 열 이름을 설정합니다.

<figure><img src="../../../../.gitbook/assets/image (1629).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364571/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092717000\&api=v2) 셀 범위를 선택하고 셀 유형을 단추로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (509).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364571/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092717000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 추가**버튼을** 클릭하면 추가 성공이 표시된 경고 상자가 나타납니다.<br>

<figure><img src="../../../../.gitbook/assets/image (1866).png" alt=""><figcaption></figcaption></figure>
