# getTableDataByCondition 메서드

### 메서드&#x20;

Forguncy.getTableDataByCondition(condition, formulaCalcContext, callBack, async)

### 설명&#x20;

조건을 통해 데이터 테이블 또는 뷰에 대한 데이터를 가져옵니다.

### 매개 변수&#x20;



<table><thead><tr><th width="206">매개변수 </th><th>형식 </th><th width="127">필요여부 </th><th>설명 </th></tr></thead><tbody><tr><td>condition</td><td><a href="https://help.grapecity.com.cn/pages/viewpage.action?pageId=72364493">GetTableDataByConditionParams</a></td><td>필수 </td><td>데이터를 가져오는 조건입니다.</td></tr><tr><td>formulaCalcContext</td><td><a href="https://help.grapecity.com.cn/pages/viewpage.action?pageId=72364491">FormulaCalcContext</a></td><td>필수 </td><td>매개 변수에 대한 쿼리 조건에 수식이 포함된 경우 수식을 사용하여 계산된 결과를 가져오는 수식 계산에 대한 컨텍스트 정보입니다.</td></tr><tr><td>callBack</td><td>function</td><td>필수 </td><td>함수를 성공적으로 콜백했습니다.</td></tr><tr><td>async</td><td>boolean</td><td>필수아</td><td>요청이 비동기인지 여부입니다.</td></tr></tbody></table>

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서는 getTableDataByCondition 메서드를 사용하여 데이터 테이블의 데이터를 가져옵니다.

```javascript
// 데이터 매개변수 가져오기
var param = {
//데이터테이블 이름 
TableName: "직원 테이블",
//필드 이름 
Columns: ["ID", "이"],
// 디자이너에서 설정한 쿼리 조건
QueryCondition: ISqlCondition,
QueryPolicy: {
Distinct: true,
QueryNullPolicy: Forguncy.QueryNullPolicy.QueryAllItemsWhenValueIsNull,
IgnoreCache: false
},
// 디자이너에서 설정한 정렬 조건
SortCondition: ISqlCondition
};
//수식 계산의 컨텍스트 정보, 획득한 매개변수의 쿼리 조건에 수식이 포함된 경우 수식 계산 결과 사용
var formulaCalcContext = {
// 수식에서 참조하는 셀 또는 셀 범위가 마스터 페이지에 있는지 여부
IsInMasterPage: false
};
//데이터 테이블의 데이터 가져오기
Forguncy.getTableDataByCondition (param, formulaCalcContext, function(dataStr){
var tableData = dataStr;
}, true);
```
