# getTabPage 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365030/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 메서드 <a href="#gettabpage-fang-fa-fang-fa" id="gettabpage-fang-fa-fang-fa"></a>

&#x20;  Cell.getTabPage(tabIndex)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365030/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 설명 <a href="#gettabpage-fang-fa-miao-shu" id="gettabpage-fang-fa-miao-shu"></a>

탭 컨테이너에서 서브 페이지 개체를 가져옵니다. 이 메서드는 셀 유형이 탭인 경우에만 사용됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365030/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **매개 변수**  <a href="#gettabpage-fang-fa-can-shu-shuo-ming" id="gettabpage-fang-fa-can-shu-shuo-ming"></a>

| 매개변수     | 형식     | 설명                  |
| -------- | ------ | ------------------- |
| tabIndex | number | 페이지 인덱스, 0부터 시작합니다. |

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365030/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **반환값**  <a href="#gettabpage-fang-fa-fan-hui-zhi" id="gettabpage-fang-fa-fan-hui-zhi"></a>

&#x20;  SubPage

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365030/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 예제 <a href="#gettabpage-fang-fa-shi-li" id="gettabpage-fang-fa-shi-li"></a>

다음 예제 코드에서는 getTabPage 메서드를 사용하여 지정된 탭(container)의 하위 페이지(페이지 1)의 셀(myCell) 값을 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 탭 가져오기
var tabControlCell = page.getCell("tabControl");
// 탭의 하위 페이지를 가져옵니다. 탭에서 셀이나 표를 가져와야 하는 경우 먼저 탭에서 하위 페이지의 정보를 가져와야 합니다. 탭 번호는 0에서 시작합니다.
var tab1 = tabControlCell.getTabPage(0);
//첫 번째 레이블에서 myCell이라는 이름의 셀을 가져옵니다.
var subPageCell = tab1.getCell("myCell");
// 셀의 값을 가져오고 경고 상자를 표시합니다.
alert(subPageCell.getValue());
```

![](https://help.grapecity.com.cn/download/thumbnails/72365030/16.png?version=1\&modificationDate=1648092723000\&api=v2) **사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365030/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092723000\&api=v2) 탭 페이지에서 셀 범위를 선택하고 탭으로 설정하고 이름을 "tabControl"로 지정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1515).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365030/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092723000\&api=v2) 페이지 1을 열고 페이지 행과 열 수를 모두 10으로 설정하고 페이지에서 셀 범위를 선택하여 myCell이라는 이름을 지정합니다. 값을 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1133).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365030/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092723000\&api=v2) 탭 페이지를 열고 선택 카드를 선택하고 셀 설정에서 하위 페이지를 페이지 1로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (537).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365030/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092723000\&api=v2) 탭 페이지에서 셀 범위를 선택하고 셀 유형을 버튼 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1264).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365030/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092723000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼 클릭하면 탭의 하위 페이지에 지정된 셀의 값이 표시되고 브라우저에 셀 값이 표시되는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (939).png" alt=""><figcaption></figcaption></figure>
