# setCustomFunction 메서드

#### 메서드 <a href="#setcustomfunction-fang-fa-fang-fa" id="setcustomfunction-fang-fa-fang-fa"></a>

&#x20;  PivotTableCellType.setCustomFunction(cellName, customFunction)&#x20;

#### 설명 <a href="#setcustomfunction-fang-fa-miao-shu" id="setcustomfunction-fang-fa-miao-shu"></a>

피벗 테이블 셀 유형의 값 요약 방법을 사용자 지정합니다.

#### **매개 변수**  <a href="#setcustomfunction-fang-fa-can-shu-shuo-ming" id="setcustomfunction-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="212.33333333333331">메서드 </th><th width="219">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>cellName</td><td>string</td><td>피벗 테이블 셀의 이름입니다.</td></tr><tr><td>customFunction</td><td>(records: any[], filedName: string) => any</td><td>선택한 필드 데이터를 요약하는 처리기입니다. 이 함수는 "records"는 요약할 데이터 집합이며 "filedName"은 요약 데이터 필드 이름이라는 두 가지 매개 변수를 허용합니다. 반환 값은 요약 결과입니다.</td></tr></tbody></table>

#### **반환값**  <a href="#setcustomfunction-fang-fa-fan-hui-zhi" id="setcustomfunction-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### 예제 <a href="#setcustomfunction-fang-fa-shi-li" id="setcustomfunction-fang-fa-shi-li"></a>

다음 예제 코드에서는 setCustomFunction 메서드를 사용 하 여 피벗 테이블 셀 형식의 값 요약 방법을 사용자 지정 합니다.

```
//페이지의 피벗 테이블 셀 가져오기
var cell = Forguncy.PivotTableCellType;
//피벗 테이블 셀 유형의 값이 요약되는 방식을 사용자 정의합니다.
cell.setCustomFunction("pivottablecell", function (records, filedName) {
 
//값 요약 메소드 정의
var count = records.length;
return count;
});
```

**절차를 따르십시오**

1. 디자이너의 페이지에서 셀 범위를 선택하고 테이블을 바인딩한 다음 피벗 테이블로 설정된 셀 범위를 선택하고 값 필드는 금액이며 합계로 요약됩니다. 이름을 "pivottablecell"으로 설정합니다.\
   실행 후 페이지는 다음과 같이 표시됩니다.

<figure><img src="../../../../../.gitbook/assets/image (395).png" alt=""><figcaption></figcaption></figure>

2. 페이지 설정에서 페이지 로드를 편집할 때의 명령은 \[자바스크립트로 직접 프로그래밍하기]이며 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1886).png" alt=""><figcaption></figcaption></figure>

3. 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.\
   페이지를 실행한 후 피벗 테이블의 값이 사용자 지정 방식으로 요약되는 것을 볼 수 있습니다.

<figure><img src="../../../../../.gitbook/assets/image (1345).png" alt=""><figcaption></figcaption></figure>
