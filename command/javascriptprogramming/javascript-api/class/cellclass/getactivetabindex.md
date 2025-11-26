# getActiveTabIndex 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364970/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) 메서드 <a href="#getactivetabindex-fang-fa-fang-fa" id="getactivetabindex-fang-fa-fang-fa"></a>

&#x20;  Cell.getActiveTabIndex()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364970/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) 설명 <a href="#getactivetabindex-fang-fa-miao-shu" id="getactivetabindex-fang-fa-miao-shu"></a>

0부터 시작하는 현재 탭의 번호를 가져옵니다. 이 메서드는 셀 유형이 탭인 경우에만 사용됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364970/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) **매개 변수** <a href="#getactivetabindex-fang-fa-can-shu-shuo-ming" id="getactivetabindex-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364970/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) **반환값**  <a href="#getactivetabindex-fang-fa-fan-hui-zhi" id="getactivetabindex-fang-fa-fan-hui-zhi"></a>

&#x20;  number

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364970/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) 예제 <a href="#getactivetabindex-fang-fa-shi-li" id="getactivetabindex-fang-fa-shi-li"></a>

다음 예제 코드에서는 getActiveTabIndex 메서드를 통해 현재 탭의 번호를 가져옵니다.

```
//현재 페이지 가져오기
var page = Forguncy.Page;
//탭 가져오기
var tabControlCell = page.getCell("tabControl");
//현재 탭의 번호를 가져옵니다. 번호 매기기는 0부터 시작합니다.
var activeTabIndex = tabControlCell.getActiveTabIndex();
//현재 탭의 번호를 보여주는 경고 상자 팝업
alert(activeTabIndex);
```

#### Forguncy 사용 예제

1. 페이지를 여러 개 생성합니다. 예제에서는 총 5개의 페이지를 생성했습니다.\
   ‘페이지2 \~ 페이지5’까지는 그림이나 텍스트 등 컨텐츠를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getactivetabindex01.png" alt=""><figcaption></figcaption></figure>

2\. ‘페이지1’에 “페이지 내 탭 컨트롤 셀” 유형의 셀을 생성합니다.\
오른쪽 ‘셀 유형’에 “탭”을 ‘페이지2 \~ 페이지5’까지 나타나도록 지정합니다.\
이후 페이지 왼쪽 위에 해당 Cell Name을 tabControl이라고 적어줍니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getactivetabindex02.png" alt=""><figcaption></figcaption></figure>

3\. 페이지 내에 버튼을 한 개 추가하고, 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getactivetabindex03.png" alt=""><figcaption></figcaption></figure>

4\. 해당 프로젝트를 실행하고 탭을 이동하면서 버튼을 클릭하면 화면에 활성화되어 있는 탭의 Tab Index 번호가 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getactivetabindex04.gif)

<br>
