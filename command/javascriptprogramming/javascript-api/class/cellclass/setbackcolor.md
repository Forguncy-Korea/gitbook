# setBackColor 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365094/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 메서드 <a href="#setbackcolor-fang-fa-fang-fa" id="setbackcolor-fang-fa-fang-fa"></a>

Cell.setBackColor(color)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365094/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 설명 <a href="#setbackcolor-fang-fa-miao-shu" id="setbackcolor-fang-fa-miao-shu"></a>

지정된 셀에 배경색을 설정합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365094/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **매개 변수** <a href="#setbackcolor-fang-fa-can-shu-shuo-ming" id="setbackcolor-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="154.33333333333331">매개변수 </th><th width="142">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>color</td><td>any </td><td><p>다음 세 가지 형식을 지원하는 색상을 설정합니다.</p><ul><li>색상 이름(예: red;</li><li>#ff0000 같은 16진수 값;</li><li>rgb 코드(예: rgb(255,0,0))입니다.</li></ul></td></tr></tbody></table>

<br>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365094/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) **반환값**  <a href="#setbackcolor-fang-fa-fan-hui-zhi" id="setbackcolor-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365094/blue%20block.png?version=1\&modificationDate=1648092724000\&api=v2) 예제 <a href="#setbackcolor-fang-fa-shi-li" id="setbackcolor-fang-fa-shi-li"></a>

다음 예제 코드에서는 setBackColor 메서드를 사용 하 여 지정 된 셀에 배경색을 설정 합니다.

```
//현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
var cell = page.getCell("myCell");
//셀의 배경색 설정
var setColor = cell.setBackColor("red");
```



#### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. “텍스트 상자” 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 myCell이라고 이름을 지정합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-setbackcolor01.png" alt=""><figcaption></figcaption></figure>

2\. 페이지에 “버튼”을 하나 생성하고, 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-setbackcolor02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하여 버튼을 클릭합니다. myCell 셀에 배경색이 더해집니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-setbackcolor03.gif)
