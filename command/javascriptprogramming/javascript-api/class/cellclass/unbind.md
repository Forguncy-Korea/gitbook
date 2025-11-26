# unbind 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365181/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) 메서드 <a href="#unbind-fang-fa-fang-fa" id="unbind-fang-fa-fang-fa"></a>

&#x20;  Cell.unbind(type, fn)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365181/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) 설명 <a href="#unbind-fang-fa-miao-shu" id="unbind-fang-fa-miao-shu"></a>

선택한 요소에 대한 이벤트 처리기를 제거합니다. 이 메서드는 선택한 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365181/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) **매개 변수** <a href="#unbind-fang-fa-can-shu-shuo-ming" id="unbind-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="125">매개변수 </th><th width="131">형식 </th><th width="114">필수여부</th><th>설명 </th></tr></thead><tbody><tr><td>type</td><td>string</td><td>Yes</td><td>이벤트 형식을 나타내는 문자열입니다. 셀에서 지원하는 이벤트는 CellEvents 클래스를 참조하십시오.</td></tr><tr><td>fn</td><td>function</td><td>No</td><td>이벤트 처리기입니다. 생략하면 해당 이벤트 형식의 셀에 대한 모든 처리기의 바인딩이 해제됩니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365181/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) **반환값**  <a href="#unbind-fang-fa-fan-hui-zhi" id="unbind-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365181/blue%20block.png?version=1\&modificationDate=1648092726000\&api=v2) 예제입니다 <a href="#unbind-fang-fa-shi-li" id="unbind-fang-fa-shi-li"></a>

다음 예제 코드에서는 unbind 메서드를 통해 버에 대한 클릭 이벤트 바인딩을 제거합니다.

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
//특정 이벤트 핸들러 바인딩 해제
cell.unbind("click", onClick);
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
