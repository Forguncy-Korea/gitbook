# setValue 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365141/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 메서드 <a href="#setvalue-fang-fa-fang-fa" id="setvalue-fang-fa-fang-fa"></a>

Cell.setValue(value)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365141/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 설명 <a href="#setvalue-fang-fa-miao-shu" id="setvalue-fang-fa-miao-shu"></a>

지정된 셀에 대한 값을 설정합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365141/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) **매개 변수**  <a href="#setvalue-fang-fa-can-shu-shuo-ming" id="setvalue-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="181.33333333333331">매개변수 </th><th width="127">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>value</td><td>any</td><td>임의의 값을 입력할 수 있는 값을 설정합니다.</td></tr></tbody></table>

<br>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365141/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) **반환값**  <a href="#setvalue-fang-fa-fan-hui-zhi" id="setvalue-fang-fa-fan-hui-zhi"></a>

any

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365141/blue%20block.png?version=1\&modificationDate=1648092725000\&api=v2) 예제 <a href="#setvalue-fang-fa-shi-li" id="setvalue-fang-fa-shi-li"></a>

다음 예제 코드에서는 setValue 메서드를 사용 하 여 지정 된 셀 (myCell)의 값을 설정 합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 myCell이라는 이름의 셀을 가져옵니다.
 var textCell = page.getCell("myCell");
//지정된 셀의 값 설정
textCell.setValue("이동 가능한 유형");
```



#### Forguncy 사용 예제

1.페이지를 한 개 생성하고, 빈 셀에 하나를 생성합니다. 이후 좌측상단의 Cell Name에 myCell이라고 입력해 줍니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-setvalue01.png" alt=""><figcaption></figcaption></figure>

2\. 버튼을 생성하여 아래와 같이 “자바스크립트로 직접 프로그래밍하기” 명령을 생성하고, 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-setvalue02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하고, 버튼을 클릭하면 myCell에 입력된 값(value)가 화면에 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-setvalue03.gif)
