# getCellArray 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365999/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 메서드 <a href="#getcellarray-fang-fa-fang-fa" id="getcellarray-fang-fa-fang-fa"></a>

Page.getCellArray(name, includeSubPage)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365999/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 설명 <a href="#getcellarray-fang-fa-miao-shu" id="getcellarray-fang-fa-miao-shu"></a>

셀 이름으로 셀 인스턴스 집합을 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365999/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) **매개 변수** <a href="#getcellarray-fang-fa-can-shu-shuo-ming" id="getcellarray-fang-fa-can-shu-shuo-ming"></a>

<table data-header-hidden><thead><tr><th width="185.33333333333331">매개변수 </th><th width="159">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>name</td><td>string</td><td>셀 이름입니다.</td></tr><tr><td>includeSubPage</td><td>Boolean</td><td>하위 페이지에서 찾을지 여부입니다. 선택적 매개 변수( 기본값은 true)입니다.</td></tr></tbody></table>

#### &#x20;![](https://help.grapecity.com.cn/download/thumbnails/72365999/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) **반환 값**  <a href="#getcellarray-fang-fa-fan-hui-zhi" id="getcellarray-fang-fa-fan-hui-zhi"></a>

&#x20;  [Cell](https://help.grapecity.com.cn/pages/viewpage.action?pageId=72364904)[\[\]](https://help.grapecity.com.cn/pages/viewpage.action?pageId=72364904)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365999/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 예제 <a href="#getcellarray-fang-fa-shi-li" id="getcellarray-fang-fa-shi-li"></a>

다음 예제 코드에서는 getCellArray 메서드를 통해 셀 인스턴스 집합을 가져오고 반환된 셀 인스턴스의 길이를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//셀 객체 가져오기
var cell = page.getCellArray("myCell");
//셀 인스턴스의 길이 가져오기
var len = cell.length;
// 셀 인스턴스의 길이를 보여주는 경고 상자 팝업
alert(len);
```

#### Forguncy 사용 예제

1.  Forguncy에서 빈 페이지 2개를 생성합니다.\
    “페이지1”에서 아래와 같이 셀 범위를 선택 > 셀 유형을 “내용이 포함된 셀 타입” 선택 > 하위 페이지로 “페이지2”를 지정합니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcellarray02.png)\
    <br>

    ※ 참고 : “내용이 포함된 셀 타입”이라는 셀 유형은 아래와 같은 위치에 있습니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcellarray01.png)\
    <br>
2.  “페이지2”로 이동하여 아래 그림과 같이 셀 영역을 설정합니다.\
    (1) 셀을 병합하지 않습니다. 여러 개의 셀을 선택한 상태로 그냥 두시면 됩니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcellarray03.png)\
    (2) 이후 영역이 선택된 상태에서 좌측 상단에 “myCell”이라고 붙여 줍니다.

    ※ 참고 : ForguncyCell Name과 관련한 사항에 대해서는 별도의 페이지에서 설명합니다.\
    <br>
3.  “페이지1”로 돌아가서 아래 그림과 같이 “버튼”을 생성하고, 버튼에 명령을 설정합니다.

    (1) 셀 영역을 선택하신 후 셀 유형을 “버튼”으로 선택합니다.

    (2) 버튼 셀을 선택 시 우측에 나타나는 패널에 “명령 편집”으로 이동합니다.

    (3) “JavaScript로 직접 프로그래밍하기” 명령을 이용하여 스크립트를 작성합니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcellarray04.png)\
    <br>
4. 프로젝트를 실행합니다.
5.  웹브라우저에서 아래와 같이 ‘버튼’을 클릭하면, 10이라는 팝업창이 나타납니다.\
    myCell로 지정된 Cell의 영역이 총 10개이므로, myCell이라는 영역의 길이는 10으로 나타납니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcellarray05.gif)

<br>
