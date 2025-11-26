# disable 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364924/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) 메서드 <a href="#disable-fang-fa-fang-fa" id="disable-fang-fa-fang-fa"></a>

Cell.disable()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364924/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) 설명 <a href="#disable-fang-fa-miao-shu" id="disable-fang-fa-miao-shu"></a>

셀을 사용하지 않도록 설정합니다. 셀이 비활성화되면 클릭할 수 없습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364924/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) **매개 변수** <a href="#disable-fang-fa-can-shu-shuo-ming" id="disable-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364924/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) **반환값**  <a href="#disable-fang-fa-fan-hui-zhi" id="disable-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364924/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) 예제 <a href="#disable-fang-fa-shi-li" id="disable-fang-fa-shi-li"></a>

다음 예제 코드에서 disable 메서드를 사용 하 여 지정된 체크박스를 사용 하지 않도록 설정 하려면 버튼 클릭 합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 이름이 checkBox인 체크박스를 가져옵니다.
var cell = page.getCell("checkBox");
// 체크박스 비활성화
cell.disable();
```

#### Forguncy 사용 예제

※참고 : disable과 enable은 한 세트이므로 같은 예제가 구성되어 있습니다.

1. 페이지를 한 개 생성하고, 체크박스 셀을 하나 생성합니다. 이후 좌측상단의 Cell Name에 checkbox라고 입력해 줍니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-disable01.png" alt=""><figcaption></figcaption></figure>

2\. 버튼을 생성하여 아래와 같이 “자바스크립트로 직접 프로그래밍하기” 명령을 생성하고, 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-disable02.png" alt=""><figcaption></figcaption></figure>

3\. 또 다른 버튼을 하나 추가로 생성하여 아래와 같이 “자바스크립트로 직접 프로그래밍하기” 명령을 생성하고, 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-disable03.png" alt=""><figcaption></figcaption></figure>

4\. 해당 프로젝트를 실행하고 체크박스를 클릭할 수 있는 지 확인합니다.\
Disable 버튼을 클릭하면 체크박스가 회색으로 변경되며, 클릭이 불가능하게 변경됩니다.\
Enable 버튼을 클릭하면 체크박스가 다시 클릭 가능한 상태로 변경됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-disable04.gif)

<br>
