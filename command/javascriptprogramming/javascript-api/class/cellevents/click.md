# Click 이벤트

#### &#x20;![](https://help.grapecity.com.cn/download/thumbnails/72364816/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 이벤트 <a href="#click-shi-jian-shi-jian" id="click-shi-jian-shi-jian"></a>

&#x20;  Forguncy.CellEvents.Click

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364816/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 설명 <a href="#click-shi-jian-miao-shu" id="click-shi-jian-miao-shu"></a>

셀을 클릭하면 버튼, 이미지 및 하이퍼링크 셀 유형을 지원하는 이벤트가 트리거됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364816/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) **반환값**  <a href="#click-shi-jian-fan-hui-zhi" id="click-shi-jian-fan-hui-zhi"></a>

String&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364816/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 예제 <a href="#click-shi-jian-shi-li" id="click-shi-jian-shi-li"></a>

다음 예제 코드에서는 bnd 메서드를 사용하여 단추에 클릭 이벤트를 추가하고 버튼을 클릭할 때 경고 상자가 나타납니다.

```
   //클릭 시 실행한 binding 함수를 정의합니다.
    var onClickEventFunction = function(arg) {

        //화면에 표시할 문구를 정의합니다.
        alert("안녕하세요. Forguncy!");
    }

    //현재 페이지에 Namespace를 선언합니다.
    var page = Forguncy.Page;
    
    //Cell Name이 button이라고 지정된 셀을 가져옵니다.
    var cell = page.getCell("button");

    //button 셀에 onClickEventFunction를 click할 때 이벤트가 발생하도록 binding합니다.
    cell.bind("click", onClickEventFunction);
```





#### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. “버튼” 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 buitton이라고 이름을 지정합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-click01.png" alt=""><figcaption></figcaption></figure>

2\. 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-click02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하여 버튼을 클릭합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-click03.gif" alt=""><figcaption></figcaption></figure>

※참고 : bind 메소드로 이벤트를 바인딩 하는 경우 binding하는 시점에는 아무 이벤트가 발생하지 않는 것처럼 보여 두 번 클릭하는 것처럼 보일 수 있습니다. 이는 첫 번 째 클릭 시에는 cell.bind가 실행되어 CallBack 함수인 onClickEventFunction 함수가 버튼에 바인딩되는 이벤트가 실행되기 때문에 실제 눈에 보이지 않아서 그렇습니다. CallBack 함수를 Binding하는 경우는 이벤트를 바인딩하는 시점에 한 스텝이 더 진행됩니다
