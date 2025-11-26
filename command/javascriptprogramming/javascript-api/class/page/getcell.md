# getCell 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366027/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 메서드 <a href="#getcell-fang-fa-fang-fa" id="getcell-fang-fa-fang-fa"></a>

&#x20;  Page.getCell(name, includeSubPage)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366027/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 설명 <a href="#getcell-fang-fa-miao-shu" id="getcell-fang-fa-miao-shu"></a>

셀 이름으로 셀 인스턴스를 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366027/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) **매개 변수** <a href="#getcell-fang-fa-can-shu-shuo-ming" id="getcell-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="197.33333333333331">매개변수 </th><th width="172">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>name</td><td>string</td><td>셀 이름입니다.</td></tr><tr><td>includeSubPage</td><td>Boolean</td><td>하위 페이지에서 찾을지 여부입니다. 선택적 매개 변수( 기본값은 true)입니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366027/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) **반환값**  <a href="#getcell-fang-fa-fan-hui-zhi" id="getcell-fang-fa-fan-hui-zhi"></a>

&#x20;  [Cell](../cellclass/)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366027/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 예제 <a href="#getcell-fang-fa-shi-li" id="getcell-fang-fa-shi-li"></a>

다음 예제 코드에서는 getCell 메서드를 통해 셀 인스턴스를 가져오고 셀 값을 설정합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//셀 객체 가져오기
var cell = page.getCell("myCell");
//셀 값 설정
cell.setValue("이동 가능한 유형");
```



#### Forguncy 사용 예제

1. Forguncy에서 페이지 2개를 생성합니다.
2. “페이지1”에 셀 범위를 선택한 후 병합합니다. “페이지 2”에도 셀 범위를 선택한 후 병합합니다.
3.  “페이지1”의 셀에는 myCell1, “페이지2”의 셀에는 myCell2라고 입력합니다. 화면 좌측 위에 입력하시면 됩니다.<br>

    <figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcell01.png" alt=""><figcaption></figcaption></figure>
4.  “페이지1”에서 아래와 같이 셀 범위를 선택 > 셀 유형을 “내용이 포함된 셀 타입” 선택 > 하위 페이지로 “페이지2”를 지정합니다.<br>

    ※ 참고 : “내용이 포함된 셀 타입”이라는 셀 유형은 아래와 같은 위치에 있습니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcellarray01.png)\
    <br>

    <figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcell03.png" alt=""><figcaption></figcaption></figure>
5.  “페이지1”에 버튼을 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.<br>

    <figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcell02.png" alt=""><figcaption></figcaption></figure>
6.  해당 프로젝트를 실행하고, 버튼을 누르면 myCell1과 myCell2에 각각 Forguncy1, Forguncy2라고 입력됩니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcell04.gif)
