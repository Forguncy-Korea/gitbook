# clearAllColumnFilters 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365900/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) 메서드 <a href="#clearallcolumnfilters-fang-fa-fang-fa" id="clearallcolumnfilters-fang-fa-fang-fa"></a>

&#x20;  ListView.clearAllColumnFilters()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365900/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) 설명 <a href="#clearallcolumnfilters-fang-fa-miao-shu" id="clearallcolumnfilters-fang-fa-miao-shu"></a>

리스트뷰의 모든 열 필터 항목을 지웁니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365900/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) **매개 변수**    <a href="#clearallcolumnfilters-fang-fa-can-shu-shuo-ming" id="clearallcolumnfilters-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365900/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) **반환값**  <a href="#clearallcolumnfilters-fang-fa-fan-hui-zhi" id="clearallcolumnfilters-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365900/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) 예제 <a href="#clearallcolumnfilters-fang-fa-shi-li" id="clearallcolumnfilters-fang-fa-shi-li"></a>

다음 예제 코드에서는 clearAllColumnFilters 메서드를 사용하여 리스트의 모든 열 필터 항목을 지웁니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트 1");
//리스트 개체의 열 필터 항목을 지웁니다.
  listview.clearAllColumnFilters();
```
