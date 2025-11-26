# showColumns 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365882/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) 메서드 <a href="#showcolumns-fang-fa-fang-fa" id="showcolumns-fang-fa-fang-fa"></a>

&#x20;  ListView.showColumns()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365882/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) 설명 <a href="#showcolumns-fang-fa-miao-shu" id="showcolumns-fang-fa-miao-shu"></a>

API 및 열 옵션 명령을 통해 숨겨진 리스트의 열을 표시합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365882/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) **매개 변수**    <a href="#showcolumns-fang-fa-can-shu-shuo-ming" id="showcolumns-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="170.33333333333331">매개변수 </th><th width="193">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>columns</td><td>string 또는 number</td><td>리스트뷰의 열 이름 또는 열 인덱스는 0부터 시작합니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365882/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) **반환값**  <a href="#showcolumns-fang-fa-fan-hui-zhi" id="showcolumns-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365882/blue%20block.png?version=1\&modificationDate=1648092737000\&api=v2) 예제 <a href="#showcolumns-fang-fa-shi-li" id="showcolumns-fang-fa-shi-li"></a>

다음 예제 코드에서는 showColumns 메서드를 통해 API 및 열 옵션 명령을 통해 리스트뷰에서 숨겨진 열을 표시합니다.

예 1:

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
// "생년월일" 및 "부서"라는 열을 표시합니다.
listview.showColumns(["생년월일", "부서"]);
```

예 2:

```
// 현재 페이지 가져오기
var page  = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("리스트뷰1");
//테이블의 두 번째 및 세 번째 열을 표시합니다.
listview.showColumns([1,2]);
```

\
![](https://help.grapecity.com.cn/download/thumbnails/72365882/16.png?version=1\&modificationDate=1648092737000\&api=v2)**사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365882/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092737000\&api=v2)페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 테이블 열의 열 이름을 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365867/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092736000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1059).png" alt=""><figcaption></figcaption></figure>



![](https://help.grapecity.com.cn/download/thumbnails/72365882/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092737000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

* 페이지를 실행하고 페이지에서 열 숨기기 버튼을 클릭하면 생년월일 및 부서 열이 숨겨집니다.

<figure><img src="../../../../../.gitbook/assets/image (1326).png" alt=""><figcaption></figcaption></figure>



* 페이지에서 열 표시 버튼을 클릭하면 숨겨진 생년월일 및 부서 열이 표시됩니다.

<figure><img src="../../../../../.gitbook/assets/image (1842).png" alt=""><figcaption></figcaption></figure>
