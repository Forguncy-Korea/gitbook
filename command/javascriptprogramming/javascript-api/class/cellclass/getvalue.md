# getValue 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365050/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 메서드 <a href="#getvalue-fang-fa-fang-fa" id="getvalue-fang-fa-fang-fa"></a>

&#x20;  Cell.getValue()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365050/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 설명 <a href="#getvalue-fang-fa-miao-shu" id="getvalue-fang-fa-miao-shu"></a>

지정된 셀의 값을 가져옵니다. 셀의 값을 가져온 후 명령과 같은 다른 곳에서 사용할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365050/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **매개 변수**  <a href="#getvalue-fang-fa-can-shu-shuo-ming" id="getvalue-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365050/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **반환값**  <a href="#getvalue-fang-fa-fan-hui-zhi" id="getvalue-fang-fa-fan-hui-zhi"></a>

&#x20;  any

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365050/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 예제입니다 <a href="#getvalue-fang-fa-shi-li" id="getvalue-fang-fa-shi-li"></a>

다음 예제 코드에서는 getValue 메서드를 통해 지정된 셀(myCell)의 값을 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
var cell = page.getCell("myCell");
// 이 셀의 값을 얻는다.
var cellValue = cell.getValue();
// 이 셀의 값을 표시하기 위해 경고 상자를 표시합니다.
alert(cellValue);
```



#### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, 셀에 텍스르를 입력합니다. 이후 좌측상단의 Cell Name에 myCell이라고 입력해 줍니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getvalue01.png" alt=""><figcaption></figcaption></figure>

2\. 버튼을 생성하여 아래와 같이 “자바스크립트로 직접 프로그래밍하기” 명령을 생성하고, 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getvalue02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하고, 버튼을 클릭하면 myCell에 입력된 값(value)가 화면에 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getvalue03.gif)
