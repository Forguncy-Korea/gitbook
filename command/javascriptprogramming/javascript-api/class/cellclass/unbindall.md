# unbindAll 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 메서드 <a href="#unbindall-fang-fa-fang-fa" id="unbindall-fang-fa-fang-fa"></a>

&#x20;  Cell.unbindAll()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 설명 <a href="#unbindall-fang-fa-miao-shu" id="unbindall-fang-fa-miao-shu"></a>

페이지의 모든 이벤트에 대한 바인딩을 제거합니다. 이 메서드는 페이지의 모든 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) **매개 변수** <a href="#unbindall-fang-fa-can-shu-shuo-ming" id="unbindall-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) **반환값**  <a href="#unbindall-fang-fa-fan-hui-zhi" id="unbindall-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 예제 <a href="#unbindall-fang-fa-shi-li" id="unbindall-fang-fa-shi-li"></a>

다음 예제 코드에서는 unbindAll 메서드를 사용하여 페이지의 모든 클릭 이벤트를 바인딩 해제합니다.

```
//클릭 이벤트 핸들러를 버튼에 바인딩
var onClick = function(arg) {
    alert("活字格");
}
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 button이라는 이름의 버튼을 가져옵니다.
var cell = page.getCell("button");
//셀의 이벤트 바인딩
cell.bind("click", onClick);
//모든 클릭 이벤트 핸들러의 바인딩 해제
cell.unbindAll();
```



#### Forguncy 사용 예제

※참고 : unbind와 unbindall은 실제 사용하는 방법은 동일하며, 페이지 내 Event Handler의 수가 얼마나 많은 가에 따라 선택적으로 사용하실 수 있습니다. 이에 따라 같은 ‘사용 예제’를 사용합니다.

1. 페이지 한 개를 생성하고, 버튼을 생성한 후 왼쪽 위 Cell Name에 button이라고 입력합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-bind01.png" alt=""><figcaption></figcaption></figure>

2\. 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-bind02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하고 버튼을 클릭하면 화면에 지정한 이벤트의 문자열이 화면에 표시됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-bind03.gif" alt=""><figcaption></figcaption></figure>

4\. 해당 버튼의 자바스크립트 명령에 unbind 코드를 추가합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-unbind04.png" alt=""><figcaption></figcaption></figure>

5\. 해당 프로젝트를 실행하고 버튼을 클릭해도 아무런 이벤트가 발생하지 않습니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-unbind05.gif)
