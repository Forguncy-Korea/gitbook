# getTableData 메서드

### 매서드&#x20;

Forguncy.getTableData(tableName, primaryKey, successCallback, errorCallback)

### 설명&#x20;

데이터베이스의 기본 키를 사용하여 데이터 테이블의 레코드를 가져옵니다.

### 매개변수&#x20;



| 매개변수            | 형식                              | 설명                                         |
| --------------- | ------------------------------- | ------------------------------------------ |
| tableName       | string                          | 데이터 테이블의 이름                                |
| errorCallback   | function( string errorMessage ) | 오류 메시지가 포함된 콜백 함수가 실패했습니다.                 |
| successCallback | function( plainObject data )    | 함수를 성공적으로 콜백했습니다.                          |
| primaryKey      | plainObject                     | 필드 이름과 값을 지정하고 지정된 값은 한 행에서만 찾을 수 있어야 합니다. |

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서는 getTableData 메서드를 통해 데이터 테이블의 데이터를 가져옵니다.

<pre class="language-javascript"><code class="lang-javascript">//데이터 테이블의 데이터 가져오기
Forguncy.getTableData("직원테이블", 
{
"ID":2
},
<strong>// 데이터를 수집을 성공하면 이름 열의 값을 표시하는 창 팝업됩니다.
</strong>function(data){           
alert(data.이름);
},
//데이터 수집에 실패하면 창 나타나 실패 정보를 표시합니다.
function(errorMessage){
alert(errorMessage);
}
);
</code></pre>

데이터 테이블에 고유한 행을 식별하기 위해 여러 열이 필요한 경우 샘플 코드는 다음과 같습니다.

```javascript
//데이터 테이블의 데이터 가져오기
Forguncy.getTableData("직원테이블",
{
"ID": 2,
"이름":"김민주"
},
// 데이터를 수집을 성공하면 이름 열의 값을 표시하는 창 팝업됩니다.
function(data){           
alert(data.부서);
},
데이터 수집에 실패하면 창이 나타나 실패 정보를 표시합니다.
function(errorMessage){
alert(errorMessage);
}
);
```

### 사용 방법&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/78807338/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1663664849000\&api=v2) 페이지에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (1474).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/78807338/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1663664849000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 데이터 가져오기 버튼을 클릭하면 가져온 데이터를 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (1145).png" alt=""><figcaption></figcaption></figure>
