# showTab 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365151/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 메서드 <a href="#showtab-fang-fa-fang-fa" id="showtab-fang-fa-fang-fa"></a>

&#x20;  Cell.showTab()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365151/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 설명 <a href="#showtab-fang-fa-miao-shu" id="showtab-fang-fa-miao-shu"></a>

표시되는 탭을 설정합니다. 예를 들어 첫 번째 탭이 기본적으로 표시되고 이 메서드를 사용하여 두 번째 탭을 표시할 수 있습니다. 이 메서드는 셀 유형이 탭인 경우에만 사용됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365151/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) **매개 변수** <a href="#showtab-fang-fa-can-shu-shuo-ming" id="showtab-fang-fa-can-shu-shuo-ming"></a>

| 매개변수     | 유형     | 설명                         |
| -------- | ------ | -------------------------- |
| tabIndex | number | 탭의 번호입니다. 탭 번호는 0부터 시작합니다. |

<br>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365151/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) **반환값**  <a href="#showtab-fang-fa-fan-hui-zhi" id="showtab-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365151/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 예제 <a href="#showtab-fang-fa-shi-li" id="showtab-fang-fa-shi-li"></a>

다음 예제 코드에서 showTab 메서드를 사용 하 여 표시 되는 탭이 첫 번째 탭에서 두 번째 탭으로 변경 됩니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 탭 가져오기
var tabControlCell = page.getCell("tabControl");
//탭 컨테이너의 현재 탭을 두 번째 탭으로 변경합니다. 탭 번호는 0부터 시작합니다.
tabControlCell.showTab(1);
```



#### Forguncy 사용 예제

1. 페이지를 여러 개 생성합니다. 예제에서는 총 5개의 페이지를 생성했습니다.\
   ‘페이지2 \~ 페이지5’까지는 그림이나 텍스트 등 컨텐츠를 입력합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getactivetabindex01.png" alt=""><figcaption></figcaption></figure>

2\. '페이지1’에 “페이지 내 탭 컨트롤 셀” 유형의 셀을 생성합니다.\
오른쪽 ‘셀 유형’에 “탭”을 ‘페이지2 \~ 페이지5’까지 나타나도록 지정합니다.\
이후 페이지 왼쪽 위에 해당 Cell Name을 tabControl이라고 적어줍니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getactivetabindex02.png" alt=""><figcaption></figcaption></figure>

3\. 페이지 내에 버튼을 한 개 추가하고, 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-showtab03.png" alt=""><figcaption></figcaption></figure>

4\. 해당 프로젝트를 실행하고 탭을 이동하면서 버튼을 클릭하면 지정한 Tab Index 탭이 활성화되어 화면에 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-showtab04.gif)
