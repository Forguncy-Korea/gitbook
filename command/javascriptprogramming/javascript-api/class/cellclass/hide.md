# hide 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365081/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 메서드 <a href="#hide-fang-fa-fang-fa" id="hide-fang-fa-fang-fa"></a>

&#x20;  Cell.hide()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365081/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 설명 <a href="#hide-fang-fa-miao-shu" id="hide-fang-fa-miao-shu"></a>

셀을 숨깁니다. 페이지에 지정된 셀을 숨기면 셀의 배경이 아닌 셀의 값, 유형 등만 숨길 수 있습니다. 보여주기 방법과는 달리 실제 요구 사항에 따라 사용할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365081/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **매개 변수** <a href="#hide-fang-fa-can-shu-shuo-ming" id="hide-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365081/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **반환값**  <a href="#hide-fang-fa-fan-hui-zhi" id="hide-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365081/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 예제 <a href="#hide-fang-fa-shi-li" id="hide-fang-fa-shi-li"></a>

다음 예제 코드에서는 hide 메서드를 통해 지정된 셀(myCell)을 숨깁니다.

```
//현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
var cell = page.getCell("myCell");
//myCell이라는 이름의 셀을 숨깁니다.
cell.hide();
```

#### Forguncy 사용 예제

※참고 : show와 hide는 한 세트이므로 같은 예제가 구성되어 있습니다.

1. 페이지를 한 개 생성하고, 아무 유형이나 선택해 셀을 하나 생성합니다. 이후 좌측상단의 Cell Name에 ‘myCell’이라고 입력해 줍니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hide01.png" alt=""><figcaption></figcaption></figure>

2\. 버튼을 생성하여 아래와 같이 “자바스크립트로 직접 프로그래밍하기” 명령을 생성하고, 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hide02.png" alt=""><figcaption></figcaption></figure>

3\. 또 다른 버튼을 추가로 생성하여 아래와 같이 “자바스크립트로 직접 프로그래밍하기” 명령을 생성하고, 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hide03.png" alt=""><figcaption></figcaption></figure>

4\. 해당 프로젝트를 실행하면 작동하는 Cell의 UI로 활성화되어 있음을 알 수 있습니다.\
이후 ‘Hide 버튼’을 클릭하면 해당 셀이 숨기기 처리되고, ‘Show 버튼’을 클릭하면 보이기 처리됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-hide04.gif)

<br>
