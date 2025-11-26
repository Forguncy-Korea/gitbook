# hideColumns 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365867/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 메서드 <a href="#hidecolumns-fang-fa-fang-fa" id="hidecolumns-fang-fa-fang-fa"></a>

&#x20;  ListView.hideColumns(columns)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365867/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 설명 <a href="#hidecolumns-fang-fa-miao-shu" id="hidecolumns-fang-fa-miao-shu"></a>

&#x20;  리스트뷰의 열을 숨깁니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365867/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) **매개 변수**  <a href="#hidecolumns-fang-fa-can-shu-shuo-ming" id="hidecolumns-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="165.33333333333331">매개변수 </th><th width="199">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>columns</td><td>string 또는 number</td><td>리스트뷰의 열 이름 또는 열 인덱스는 0부터 시작합니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365867/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) **반환값**  <a href="#hidecolumns-fang-fa-fan-hui-zhi" id="hidecolumns-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365867/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 예제 <a href="#hidecolumns-fang-fa-shi-li" id="hidecolumns-fang-fa-shi-li"></a>

다음 예제 코드에서는 hideColumns 메서드를 통해 리스트의 열을 숨깁니다.

예 1:

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("리스트뷰1");
// "생년월일" 및 "부서"라는 열을 숨깁니다.
listview.hideColumns(["생년월일", "부서"]);
```

예2:&#x20;

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트  가져오기
var listview = page.getListView("리스트뷰1");
// 테이블의 두 번째 및 세 번째 열을 숨깁니다.
listview.hideColumns([1,2]);
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365867/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 사용 예제 <a href="#hidecolumns-fang-fa-shi-li" id="hidecolumns-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365867/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092736000\&api=v2)페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 테이블 열의 열 이름을 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365867/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092736000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1388).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365867/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092736000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다. 페이지를 실행하고 페이지에서 열 숨기기 버튼을 클릭하면 생년월일 및 부서 열이 숨겨집니다.

<figure><img src="../../../../../.gitbook/assets/image (1482).png" alt=""><figcaption></figcaption></figure>
