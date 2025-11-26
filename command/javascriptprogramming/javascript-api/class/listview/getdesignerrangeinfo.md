# getDesignerRangeInfo 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365498/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) 메서드입니다 <a href="#getdesignerrangeinfo-fang-fa-fang-fa" id="getdesignerrangeinfo-fang-fa-fang-fa"></a>

&#x20;  ListView.getDesignerRangeInfo()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365498/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) 설명입니다 <a href="#getdesignerrangeinfo-fang-fa-miao-shu" id="getdesignerrangeinfo-fang-fa-miao-shu"></a>

시작 행 인덱스, 시작 열 인덱스, 테이블 행 수 및 열 수를 포함하여 디자이너에서 리스트 위치 정보를 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365498/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) **매개 변수**  <a href="#getdesignerrangeinfo-fang-fa-can-shu-shuo-ming" id="getdesignerrangeinfo-fang-fa-can-shu-shuo-ming"></a>

아니요, 없습니다

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365498/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) **반환값**  <a href="#getdesignerrangeinfo-fang-fa-fan-hui-zhi" id="getdesignerrangeinfo-fang-fa-fan-hui-zhi"></a>

&#x20;  CellRange

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365498/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) 예제 <a href="#getdesignerrangeinfo-fang-fa-shi-li" id="getdesignerrangeinfo-fang-fa-shi-li"></a>

다음 예제 코드에서는 getDesignerRangeInfo 메서드를 사용하여 시작 행 인덱스, 시작 열 인덱스, 리스트뷰 행 수 및 열 수를 포함하여 디자이너에서 리스트뷰 위치 정보를 가져옵니다. 행 및 열 인덱스는 0부터 시작합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
//디자이너에서 리스트의 위치 정보 가져오기
var range = listview.getDesignerRangeInfo();
// 리스트의 위치 정보를 표시하는 프롬프트 상자를 팝업합니다.
alert( "시작 행 인덱스："+range.Row+"\n"+"시작 열 인덱스："+range.Column+"\n"+"테이블의 행 수："+range.RowCount+"\n"+"테이블의 열 수："+range.ColumnCount);
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365498/blue%20block.png?version=1\&modificationDate=1648092730000\&api=v2) 사 예제 <a href="#getdesignerrangeinfo-fang-fa-shi-li" id="getdesignerrangeinfo-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365498/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092730000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365498/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092730000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1381).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365498/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092730000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 테이블 위치 정보 버튼을 클릭하면 시작 행 인덱스, 시작 열 인덱스, 테이블 행 수 및 열 수를 포함하여 디자이너에서 테이블 위치 정보가 표시되는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1026).png" alt=""><figcaption></figcaption></figure>
