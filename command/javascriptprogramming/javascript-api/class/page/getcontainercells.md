# getContainerCells 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366043/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 메서드 <a href="#getcontainercells-fang-fa-fang-fa" id="getcontainercells-fang-fa-fang-fa"></a>

&#x20;  Page.getContainerCells(includeSubPage)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366043/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 설명 <a href="#getcontainercells-fang-fa-miao-shu" id="getcontainercells-fang-fa-miao-shu"></a>

&#x20;  모든 탭 및 페이지 컨테이너 유형의 셀을 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366043/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) **매개 변수** <a href="#getcontainercells-fang-fa-can-shu-shuo-ming" id="getcontainercells-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="175.33333333333331">매개변수 </th><th width="156">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>includeSubPage</td><td>Boolean</td><td>하위 페이지에서 찾을지 여부입니다. 선택적 매개 변수( 기본값은 true)입니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366043/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) **반환값**  <a href="#getcontainercells-fang-fa-fan-hui-zhi" id="getcontainercells-fang-fa-fan-hui-zhi"></a>

&#x20;  Cell\[]

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366043/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 예제 <a href="#getcontainercells-fang-fa-shi-li" id="getcontainercells-fang-fa-shi-li"></a>

다음 예제 코드에서는 getContainerCells 메서드를 통해 셀 인스턴스 집합을 가져오고 반환된 셀 인스턴스의 길이를 가져옵니다.

```
// 현재 페이지 가져오기
var page  = Forguncy.Page;
//셀 객체 가져오기
var 셀 = page.getContainerCells();
//셀 인스턴스의 길이 가져오기
var len = cell.length;
// 셀 인스턴스의 길이를 보여주는 경고 상자 팝업
alert(len);
```

#### Forguncy 사용 예제

1. Forguncy에서 페이지 2개를 생성합니다.
2.  “페이지2”에 아무 내용이나 입력합니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcontainercells01.png)\
    <br>
3.  “페이지1”에 “페이지 내 탭 컨트롤 셀”과 “내용이 포함된 셀 타입”을 지정하고, 해당 셀의 내용으로 “페이지2”를 지정합니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcontainercells02.png)\
    <br>

    ※ 참고 : 위에서 사용한 셀 유형은 아래와 같은 위치에 있습니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcontainercells04.png)\
    <br>
4.  “페이지1”에 버튼을 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.

    <br>

    <figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcontainercells03.png" alt=""><figcaption></figcaption></figure>
5.  해당 프로젝트를 실행하고, 버튼을 누르면 getContinerCells는 두 개의 셀 유형을 감지하여 2를 보여줍니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getcontainercells05.gif)

<br>
