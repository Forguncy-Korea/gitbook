# updateTableData 메서드

### 메서드&#x20;

Forguncy.updateTableData(tableName, primaryKey, updateValue, successCallback, errorCallback)

### 설명&#x20;

primaryKey 매개 변수를 사용하여 업데이트할 레코드의 고유한 행을 지정합니다.

### 매개변수&#x20;



| 매개변수            | 형식          | 설명                                                                      |
| --------------- | ----------- | ----------------------------------------------------------------------- |
| tableName       | string      | 레코드를 업데이트할 데이터 테이블의 테이블 이름입니다.                                          |
| primaryKey      | plainObject | 레코드를 수정할 필드 이름과 값을 지정하려면 지정된 값에 대해 하나의 행만 찾을 수 있어야 합니다.                 |
| updateValue     | plainObject | 업데이트된 값을 나타내는 개체, 업데이트할 값을 나타내는 개체의 속성입니다. 데이터 테이블의 모든 열을 포함할 필요는 없습니다. |
| successCallback | function    | 수정된 행의 값을 포함하는 인수가 있는 함수가 성공적으로 콜백되었습니다.                                |
| errorCallback   | function    | 매개 변수에 오류 메시지가 포함된 콜백 함수가 실패했습니다.                                       |

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서는 updateTableData 메서드를 통해 데이터 테이블의 데이터를 업데이트합니다.

```
//데이터 테이블의 데이터 업데이트
Forguncy.updateTableData("직원테이블",{"ID":1},
{
이름: "리틀 리",
부서: "개발 부서"
},
//업데이트가 성공하면 업데이트가 성공했다는 경고창이 뜹니다.
function(data){          
alert("업데이트 성공！");
},
//업데이트 데이터가 실패하면 경고 상자가 나타나 실패 정보를 보여줍니다.
function(errorMessage){
alert(errorMessage);
}
);
```

데이터 테이블에 고유한 행을 식별하기 위해 여러 열이 필요한 경우 샘플 코드는 다음과 같습니다.

```
//데이터 테이블의 데이터 업데이트
Forguncy.updateTableData("직원테이블",{"ID":1, "이름": "김남"},
{
부서: "개발 부서"
},
//업데이트가 성공하면 업데이트가 성공했다는 경고창이 뜹니다.
function(data){
alert("업데이트 성공!");
},
//업데이트 데이터가 실패하면 경고 상자가 나타나 실패 정보를 보여줍니다.
function(errorMessage){
alert(errorMessage);
}
);
```

\[옵션-> 응용 프로그램 실행]에서 "JavaScript Api를 사용하여 데이터베이스에 접근하여 내용을 변경할 수 없습니다." 선택하면 이 메서드를 사용하여 지정된 데이터 테이블에 데이터를 추가할 때 실패합니다. 이 메서드를 사용 하 여이 메서드를 사용 하 여이 작업을 수행 하기 전에이 옵션을 선택 취소 합니다.

<figure><img src="../../../../.gitbook/assets/image (2181).png" alt=""><figcaption></figcaption></figure>

### 사용 예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364791/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092720000\&api=v2) 페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72364791/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092720000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (1602).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364791/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092720000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 업데이트 버튼을 클릭하면 업데이트가 성공한다는 경고 상자가 나타납니다.
