# Page 변수

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366517/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 설명 <a href="#page-bian-liang-miao-shu" id="page-bian-liang-miao-shu"></a>

포건시의 루트 개체인 페이지 개체는 페이지 개체를 통해 셀 개체 및 테이블 개체를 가져올 수 있습니다. 페이지의 셀과 테이블은 현재 페이지로 가져온 경우에만 조작할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366517/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 형식입니다 <a href="#page-bian-liang-lei-xing" id="page-bian-liang-lei-xing"></a>

&#x20;  [Page](page/)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366517/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 예제 <a href="#page-bian-liang-shi-li" id="page-bian-liang-shi-li"></a>

예 1: 페이지 개체를 통해 셀 개체를 가져옵니다.

셀 개체를 가져오면 셀 개체에 대한 여러 메서드를 구현할 수 있습니다. 자세한 내용은 [Cell 클래스](cellclass/)를 참조하십시오

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 button이라는 이름의 버튼을 가져옵니다.
var cell = page.getCell("button");
```

예 2: 페이지 개체를 통해 테이블 개체를 가져옵니다.

테이블 개체를 가져오면 테이블 개체를 구현하는 여러 가지 방법이 있습니다. 자세한 내용은 [ListView 클래스](listview/)를 참조하십시오.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트뷰 가져오기 
var listview = page.getListView("리스트뷰1");
```
