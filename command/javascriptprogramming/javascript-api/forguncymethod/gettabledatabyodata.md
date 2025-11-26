# getTableDataByOData 메서드

### 매서드&#x20;

Forguncy.getTableDataByOData(odataParam, successCallback, errorCallback, async: boolean)

### 설명&#x20;

OData 쿼리 문자열을 통해 데이터를 가져옵니다.

### 매개변수&#x20;



<table><thead><tr><th>매개변수 </th><th>형식 </th><th width="79">필수여부 </th><th>설명 </th></tr></thead><tbody><tr><td>odataParam</td><td>string</td><td>Yes</td><td>OData 쿼리 문자열입니다.</td></tr><tr><td>successCallback</td><td>function( plainObject data )</td><td>Yes</td><td>함수를 성공적으로 콜백했습니다.</td></tr><tr><td>errorCallback</td><td>function( string errorMessage )</td><td>Yes</td><td>오류 메시지가 포함된 콜백  실패</td></tr><tr><td>async</td><td>boolean</td><td>No</td><td>요청이 비동기인지 여부</td></tr></tbody></table>

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

```javascript
//OData 쿼리 문자열을 통해 데이터 가져오기
Forguncy.getTableDataByOData("직원테이블?$select=*&$filter=ID ge 3",
function(data){
for(var i = 0; i < data.length; i++)
{
var id = data[i]["ID"];
var name = data[i]["이름"];
alert("ID=" + id + "; Name=" + name);
}
},
// 실패했을 경우 
function(errorMessage){
alert(errorMessage);
}
);
```

![](https://help.grapecity.com.cn/download/thumbnails/78807365/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1663665336000\&api=v2) 페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 각 열의 열 이름을 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/78807365/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1663665336000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (941).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/78807365/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1663665336000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 데이터 가져오기 버튼을 클릭하면 가져온 데이터를 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (613).png" alt=""><figcaption></figcaption></figure>
