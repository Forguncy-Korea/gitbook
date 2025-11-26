# clearAllSelectedRows 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365438/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 메서드 <a href="#clearallselectedrows-fang-fa-fang-fa" id="clearallselectedrows-fang-fa-fang-fa"></a>

&#x20;  ListView.clearAllSelectedRows()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365438/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 설명 <a href="#clearallselectedrows-fang-fa-miao-shu" id="clearallselectedrows-fang-fa-miao-shu"></a>

리스트에서 선택한 모든 행의 선택을 취소합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365438/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **매개 변수** <a href="#clearallselectedrows-fang-fa-can-shu-shuo-ming" id="clearallselectedrows-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365438/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **반환값**  <a href="#clearallselectedrows-fang-fa-fan-hui-zhi" id="clearallselectedrows-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365438/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 예제 <a href="#clearallselectedrows-fang-fa-shi-li" id="clearallselectedrows-fang-fa-shi-li"></a>

다음 예제 코드에서는 clearAllSelectedRows 메서드를 사용하여 테이블에서 선택한 모든 행의 선택을 취소합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
// 선택한 모든 행의 선택을 취소합니다.
listview.clearAllSelectedRows();
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365438/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 사용 예제  <a href="#clearallselectedrows-fang-fa-shi-li" id="clearallselectedrows-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365438/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092729000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365438/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092729000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼을 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1281).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365438/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092729000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 여러 행의 데이터를 선택한 다음 선택 취소 버튼 클릭하면 선택한 모든 행의 선택이 취소됩니다.

<figure><img src="../../../../../.gitbook/assets/image (431).png" alt=""><figcaption></figcaption></figure>

