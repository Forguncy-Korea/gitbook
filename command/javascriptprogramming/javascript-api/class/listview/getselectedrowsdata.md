# getSelectedRowsData 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365600/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 메서드 <a href="#getselectedrowsdata-fang-fa-fang-fa" id="getselectedrowsdata-fang-fa-fang-fa"></a>

ListView. getSelectedRowsData()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365600/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 설명 <a href="#getselectedrowsdata-fang-fa-miao-shu" id="getselectedrowsdata-fang-fa-miao-shu"></a>

리스트 선택 행에 대한 데이터를 가져옵니다. 여기에는 행의 행 인덱스, 쿼리 조건 및 데이터 선택이 포함됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365600/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) **매개 변수** <a href="#getselectedrowsdata-fang-fa-can-shu-shuo-ming" id="getselectedrowsdata-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365600/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) **반환값**  <a href="#getselectedrowsdata-fang-fa-fan-hui-zhi" id="getselectedrowsdata-fang-fa-fan-hui-zhi"></a>

반환 값은 배열 RowData입니다.

```
class RowData {
// 테이블에서 선택된 행의 행 인덱스. 행에 Query 정보가 있는 경우 RowIndex는 -1이며, 해당 행에 Query 정보가 없는 경우(예: 새 행)에만 RowIndex가 유효한 값입니다.
RowIndex: number;
RowIndex: 숫자;
//선택된 행의 쿼리 조건은 기본 키 이름을 기본 키로 사용하고 해당 데이터를 값으로 사용합니다. 예: {ID:1}
Query: object;
//선택된 행의 데이터
Values: any[];
}
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365600/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 예제 <a href="#getselectedrowsdata-fang-fa-shi-li" id="getselectedrowsdata-fang-fa-shi-li"></a>

다음 예제 코드에서는 getSelectedRowsData 메서드를 사용하여 리스트 선택 행에 대한 데이터를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
//리스트 선택 행 데이터 가져오기
var rows = listview.getSelectedRowsData();
// 리스트뷰에서 선택된 행의 정보를 표시하기 위해 경고 상자를 팝업합니다.
alert(JSON.stringify(rows, null, " "));
```

![](https://help.grapecity.com.cn/download/thumbnails/72365600/16.png?version=1\&modificationDate=1648092732000\&api=v2) **사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365600/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092732000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365600/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092732000\&api=v2)셀 범위를 선택하고 셀 유형을 단추로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (692).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365600/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092732000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 테이블에서 데이터 행을 선택한 다음 행 정보 선택 버튼을 클릭하면 행 선택 인덱스, 쿼리 조건 및 데이터를 포함하여 테이블 선택 행에 대한 정보가 포함된 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (544).png" alt=""><figcaption></figcaption></figure>
