# deleteTableData 메서드

### 메서드&#x20;

Forguncy.deleteTableData(tableName, primaryKey, successCallback, errorCallback)

### 설명&#x20;

primaryKey 매개 변수를 통해 지정된 고유 레코드를 삭제합니다.

### 매개변수&#x20;



| 매개변수            | 형식          | 설명                                         |
| --------------- | ----------- | ------------------------------------------ |
| tableName       | string      | 레코드를 삭제할 데이터 테이블의 테이블 이름입니다.               |
| primaryKey      | plainObject | 필드 이름과 값을 지정하고 지정된 값은 레코드 행만 찾을 수 있어야 합니다. |
| successCallback | function    | 함수를 성공적으로 콜백했습니다.                          |
| errorCallback   | function    | 매개 변수에 오류 메시지가 포함된 콜백 함수가 실패했습니다.          |

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서는 deleteTableData 메서드를 통해 지정된 고유 레코드를 삭제합니다.

```javascript
// 데이터 테이블에서 지정된 레코드 삭제
Forguncy.deleteTableData("직원테이블",
{
"ID": 2
},
//삭제가 성공하면 추가가 성공했다는 경고창이 뜹니다.
function () {
alert("성공적으로 삭제되었습니다.");
},
//삭제에 실패하면 경고창이 뜨면서 실패 정보를 보여줍니다.
function (errorMessage) {
alert(errorMessage);
}
);
```

데이터 테이블에 고유한 행을 식별하기 위해 여러 열이 필요한 경우 샘플 코드는 다음과 같습니다.

```
// 데이터 테이블에서 지정된 레코드 삭제
Forguncy.deleteTableData("직원테이블",
{
"ID": 2,
"이름":"한"
},
//삭제가 성공하면 추가가 성공했다는 경고창이 뜹니다.
function () {
alert("성공적으로 삭제되었습니다.");
},
//삭제에 실패하면 경고창이 뜨면서 실패 정보를 보여줍니다.
function (errorMessage) {
alert(errorMessage);
}
);
```

{% hint style="info" %}
\[옵션-> 응용 프로그램 실행]에서 "JavaScript Api를 사용하여 데이터베이스에 접근하여 내용을 변경할 수 없습니다." 선택하면 이 메서드를 사용하여 지정된 데이터 테이블에 데이터를 추가할 때 실패합니다. 이 메서드를 사용 하 여이 메서드를 사용 하 여이 작업을 수행 하기 전에이 옵션을 선택 취소 합니다.

![](<../../../../.gitbook/assets/image (2181).png>)
{% endhint %}

### 사용예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364626/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092718000\&api=v2) 페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 각 열의 열 이름을 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72364626/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092718000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.<br>

<figure><img src="../../../../.gitbook/assets/image (1197).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364626/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092718000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 삭제 버튼 클릭하면 삭제가 성공한다는 경고 상자가 나타납니다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (511).png" alt=""><figcaption></figcaption></figure>

