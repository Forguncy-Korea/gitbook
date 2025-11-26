# goToNextPage 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365670/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 메서드 <a href="#gotonextpage-fang-fa-fang-fa" id="gotonextpage-fang-fa-fang-fa"></a>

&#x20;  ListView.goToNextPage()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365670/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 설명 <a href="#gotonextpage-fang-fa-miao-shu" id="gotonextpage-fang-fa-miao-shu"></a>

리스트뷰 페이지 매김 탐색 버튼을 사용하여 리스트 데이터를 페이징하는 경우 이 방법을 사용하면 리스트뷰 현재 페이지의 다음 페이지로 이동하여 다음 페이지의 데이터를 표시할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365670/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) **매개 변수** <a href="#gotonextpage-fang-fa-can-shu-shuo-ming" id="gotonextpage-fang-fa-can-shu-shuo-ming"></a>

&#x20;  없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365670/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) **반환값**  <a href="#gotonextpage-fang-fa-fan-hui-zhi" id="gotonextpage-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365670/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 예제 <a href="#gotonextpage-fang-fa-shi-li" id="gotonextpage-fang-fa-shi-li"></a>

다음 예제 코드에서 goToNextPage 메서드를 사용 하 여 표시 되는 리스트뷰 이터는 현재 페이지의 다음 페이지로 이동 합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
// 리스트의 현재 페이지의 다음 페이지로 이동
listview.goToNextPage()
```

\
![](https://help.grapecity.com.cn/download/thumbnails/72365670/16.png?version=1\&modificationDate=1648092733000\&api=v2)**사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365670/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092733000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365640/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092732000\&api=v2)셀 범위를 선택하고 셀 유형을 페이지 탐색 버튼로 설정하고  페이징 리스트뷰 이름을 리스트뷰로설정하고 페이지당 행 수를 3개로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1793).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365670/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092733000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (362).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365670/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092733000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하면 테이블이 기본적으로 첫 번째 페이지의 데이터를 표시하고 다음 페이지 버튼을 클릭하면 두 번째 페이지로 이동합니다.

<figure><img src="../../../../../.gitbook/assets/image (2113).png" alt=""><figcaption></figcaption></figure>
