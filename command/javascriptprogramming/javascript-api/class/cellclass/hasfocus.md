# hasFocus 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365063/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 메서드 <a href="#hasfocus-fang-fa-fang-fa" id="hasfocus-fang-fa-fang-fa"></a>

&#x20;  Cell.hasFocus()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365063/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 설명 <a href="#hasfocus-fang-fa-miao-shu" id="hasfocus-fang-fa-miao-shu"></a>

지정된 셀에 포커스가 있는지 여부를 가져옵니다. 페이지의 셀 중 하나가 포커스를 가져오는지 여부를 감지하는 데 사용할 수 있습니다. 반환 값은 true 또는 false

true: 셀은 포커스를 가져옵니다.&#x20;

false: 셀이 포커스를 가져오지 않습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365063/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **반환값**  <a href="#hasfocus-fang-fa-fan-hui-zhi" id="hasfocus-fang-fa-fan-hui-zhi"></a>

boolean

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365063/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 예제입니다 <a href="#hasfocus-fang-fa-shi-li" id="hasfocus-fang-fa-shi-li"></a>

다음 예제 코드에서는 hasFocus 메서드를 사용하여 지정된 셀(myCell)에 포커스가 있는지 여부를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
var cell = page.getCell("myCell");
//현재 셀에 포커스가 있는지 확인
var f = cell.hasFocus();
// 지정된 셀에 포커스가 있는지 여부를 표시하는 경고 상자 팝업
alert(f)
```



#### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. “텍스트 상자” 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 myCell이라고 이름을 지정합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hasfocus01.png" alt=""><figcaption></figcaption></figure>

2\. 페이지에 “버튼”을 하나 생성하고, 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hasfocus02.png" alt=""><figcaption></figcaption></figure>

3\. 페이지에 “텍스트 상자”를 하나 생성하고, 해당 텍스트 상자 셀에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.\
※참고 : “텍스트 상자”에 입력한 명령은 사용자가 테스트 상자에 무언가를 입력하고나서 focus out되는 시점에 실행됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hasfocus03.png" alt=""><figcaption></figcaption></figure>

4\. 해당 프로젝트를 실행합니다.\
(1) 버튼을 클릭하면, 버튼에 focus가 오게 되므로 return되는 값은 false로 나타납니다.\
(2) 다음은 두 번 째로 생성한 텍스트 상자에 아무 값이나 입력합니다. 이후 첫 번 째 텍스트 상자를 클릭하면, 두 번 째 텍스트 상자에 입력된 명령이 실행됩니다. 첫 번 째 상자를 클릭항여 focus 상태를 이동시켰으므로, focus는 첫 번 째 텍스트 상자에 있게 되고 return되는 값은 ture로 나타납니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hasfocus04.gif)
