# usePaginationDisplay 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365852/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 메서드 <a href="#usepaginationdisplay-fang-fa-fang-fa" id="usepaginationdisplay-fang-fa-fang-fa"></a>

&#x20;  ListView.usePaginationDisplay(pageRowCount, pageIndex)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365852/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 설명 <a href="#usepaginationdisplay-fang-fa-miao-shu" id="usepaginationdisplay-fang-fa-miao-shu"></a>

이 메서드를 사용 하 여 리스트뷰에 데이터를 페이징 하 고 페이지 당 표시할 행 수를 설정 하 고 지정 된 페이지 번호로 이동할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365852/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) **매개 변수 설명입니다** <a href="#usepaginationdisplay-fang-fa-can-shu-shuo-ming" id="usepaginationdisplay-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="192">매개변수 </th><th width="102">형식</th><th width="97">필수여부</th><th>설명 </th></tr></thead><tbody><tr><td>pageRowCount</td><td>number</td><td>Yes</td><td>페이지당 표시되는 행 수입니다.</td></tr><tr><td>pageIndex</td><td>number</td><td>No</td><td>표시된 페이지의 인덱스이며 무시하면 첫 번째 페이지로 이동합니다.</td></tr></tbody></table>

#### &#x20;![](https://help.grapecity.com.cn/download/thumbnails/72365852/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) **반환값**  <a href="#usepaginationdisplay-fang-fa-fan-hui-zhi" id="usepaginationdisplay-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365852/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 예제 <a href="#usepaginationdisplay-fang-fa-shi-li" id="usepaginationdisplay-fang-fa-shi-li"></a>

다음 예제 코드에서는 usePaginationDisplay 메서드를 사용하여 페이지당 표시할 행 수를 설정하고 지정된 페이지 번호로 이동합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
//각 페이지에 표시되는 줄 수를 설정하고 지정된 페이지 번호를 입력합니다.
listview.usePaginationDisplay(6, 2)
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365852/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 사용 예제 <a href="#usepaginationdisplay-fang-fa-shi-li" id="usepaginationdisplay-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365852/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092736000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365640/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092732000\&api=v2)셀 범위를 선택하고 셀 유형을 페이지 탐색 버튼로 설정하고  페이징 리스트뷰 이름을 리스트뷰로설정하고 페이지당 행 수를 3개로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (682).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365852/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092736000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (685).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365852/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092736000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 페이지 나누기 설정 버튼을 누르면 페이지당 표시할 행 수가 설정되고 지정된 페이지 번호로 이동합니다.

<figure><img src="../../../../../.gitbook/assets/image (1382).png" alt=""><figcaption></figcaption></figure>

