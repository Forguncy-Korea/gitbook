# setFocus 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365112/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 메서드 <a href="#setfocus-fang-fa-fang-fa" id="setfocus-fang-fa-fang-fa"></a>

Cell.setFocus()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365112/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 설명 <a href="#setfocus-fang-fa-miao-shu" id="setfocus-fang-fa-miao-shu"></a>

지정된 셀에 포커스를 설정합니다. 일반적으로 셀은 마우스 클릭으로 요소를 선택하거나 탭 키를 통해 셀에 배치될 때 포커스를 받습니다. setFocus 메서드를 사용하면 지정된 셀에 직접 포커스를 부여할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365112/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) **매개 변수** <a href="#setfocus-fang-fa-can-shu-shuo-ming" id="setfocus-fang-fa-can-shu-shuo-ming"></a>

없음

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365112/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) **반환값**  <a href="#setfocus-fang-fa-fan-hui-zhi" id="setfocus-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365112/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 예제 <a href="#setfocus-fang-fa-shi-li" id="setfocus-fang-fa-shi-li"></a>

다음 예제 코드에서는 setFocus 메서드를 사용하여 셀에 포커스를 설정합니다.

```
//현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
var cell = page.getCell("myCell");
//포커스를 myCell 셀로 설정
cell.setFocus();
```

#### Forguncy 사용 예제

1.페이지 한 개 생성합니다. “텍스트 상자” 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 myCell이라고 이름을 지정합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hasfocus01.png" alt=""><figcaption></figcaption></figure>

2\. 페이지에 “버튼”을 하나 생성하고, 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-setfocus02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행합니다. “텍스트 상자”와 “버튼”이 나타나며, 둘 중 어디에도 Focus는 없는 상태입니다.\
버튼을 클릭하면 텍스트 상자에 Focus가 이동하며, 커서가 깜빡거리는 모습을 관찰할 수 있습니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-setfocus03.gif)

<br>
