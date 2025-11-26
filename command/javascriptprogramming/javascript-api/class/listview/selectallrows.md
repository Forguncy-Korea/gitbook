# selectAllRows 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365756/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 메서드 <a href="#selectallrows-fang-fa-fang-fa" id="selectallrows-fang-fa-fang-fa"></a>

&#x20;  ListView.selectAllRows()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365756/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 설명 <a href="#selectallrows-fang-fa-miao-shu" id="selectallrows-fang-fa-miao-shu"></a>

리스트뷰의 모든 행을 선택합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365756/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) **매개 변수**  <a href="#selectallrows-fang-fa-can-shu-shuo-ming" id="selectallrows-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365756/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) **반환값**  <a href="#selectallrows-fang-fa-fan-hui-zhi" id="selectallrows-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365756/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 예제 <a href="#selectallrows-fang-fa-shi-li" id="selectallrows-fang-fa-shi-li"></a>

다음 예제 코드에서 selectAllRows 메서드를 사용 하 여 리스트뷰의 모든 행을 선택 합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("리스트뷰1");
//리스트의 모든 행 선택
listview.selectAllRows();
```

\
![](https://help.grapecity.com.cn/download/thumbnails/72365756/16.png?version=1\&modificationDate=1648092734000\&api=v2)사용 예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365756/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092734000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365756/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092734000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1983).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365756/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092734000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 모든 행 선택 버튼을 클릭하면 테이블의 모든 행이 선택됩니다.

<figure><img src="../../../../../.gitbook/assets/image (1120).png" alt=""><figcaption></figcaption></figure>
