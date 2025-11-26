# goToSpecifiedPage 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365698/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 메서드 <a href="#gotospecifiedpage-fang-fa-fang-fa" id="gotospecifiedpage-fang-fa-fang-fa"></a>

&#x20;  ListView.goToSpecifiedPage(pageIndex)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365698/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 설명 <a href="#gotospecifiedpage-fang-fa-miao-shu" id="gotospecifiedpage-fang-fa-miao-shu"></a>

테이블이 페이지 매김 탐색 버튼을 사용하여 리스트를 페이징하는 경우 이 방법을 사용하면 리스트뷰가 지정된 페이지로 이동하여 지정된 페이지의 데이터를 표시할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365698/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) **매개 변수**  <a href="#gotospecifiedpage-fang-fa-can-shu-shuo-ming" id="gotospecifiedpage-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="184.33333333333331">매개변수 </th><th width="188">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>pageIndex</td><td>number</td><td>지정된 페이지 인덱스입니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365698/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) **반환값**  <a href="#gotospecifiedpage-fang-fa-fan-hui-zhi" id="gotospecifiedpage-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365698/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 예제 <a href="#gotospecifiedpage-fang-fa-shi-li" id="gotospecifiedpage-fang-fa-shi-li"></a>

다음 예제 코드에서는 goToSpecifiedPage 메서드를 사용하여 리스트뷰 지정된 페이지로 이동합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("리스트뷰1");
// 지정된 페이지로 이동
listview.goToSpecifiedPage(3)
```

#### 사용 예제 <a href="#gotospecifiedpage-fang-fa-shi-li" id="gotospecifiedpage-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365698/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092733000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365640/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092732000\&api=v2)셀 범위를 선택하고 셀 유형을 페이지 탐색 버튼로 설정하고  페이징 리스트뷰 이름을 리스트뷰로설정하고 페이지당 행 수를 3개로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (682).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365670/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092733000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1378).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365698/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092733000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하면 테이블이 기본적으로 첫 번째 페이지의 데이터를 표시하고 페이지 지정 버튼을 누르면 세 번째 페이지로 이동합니다.

<figure><img src="../../../../../.gitbook/assets/image (382).png" alt=""><figcaption></figcaption></figure>
