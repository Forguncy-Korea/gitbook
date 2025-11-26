# bind 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364906/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) 메서드 <a href="#bind-fang-fa-fang-fa" id="bind-fang-fa-fang-fa"></a>

&#x20;  Cell.bind(type, data, fn)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364906/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) 설명 <a href="#bind-fang-fa-miao-shu" id="bind-fang-fa-miao-shu"></a>

&#x20;  선택한 셀에 하나 이상의 이벤트 처리기를 추가하고 이벤트가 발생할 때 실행되는 함수를 지정합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364906/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) **매개 변수**  <a href="#bind-fang-fa-can-shu-shuo-ming" id="bind-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="115">매개변수 </th><th width="109">형식 </th><th width="117">필수여부 </th><th>설명 </th></tr></thead><tbody><tr><td>type</td><td>string</td><td>Yes</td><td>이벤트 형식을 나타내는 문자열입니다. 셀에서 지원하는 이벤트는 CellEvents 클래스 를 참조하십시오.</td></tr><tr><td>data</td><td>any</td><td>No</td><td>이벤트 처리기에 전달된 사용자 지정 매개 변수를 무시하지 않는 경우 선택적 매개 변수입니다.</td></tr><tr><td>fn</td><td>function</td><td>Yes</td><td>이벤트 처리기입니다.</td></tr></tbody></table>

<br>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364906/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) **반환값**  <a href="#bind-fang-fa-fan-hui-zhi" id="bind-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364906/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) 예제 <a href="#bind-fang-fa-shi-li" id="bind-fang-fa-shi-li"></a>

다음 예제 코드에서는 bnd 메서드를 사용하여 단추에 클릭 이벤트를 추가하고 버튼을 클릭할 때 경고 상자가 나타납니다.

예제 1.&#x20;

```
//클릭 이벤트 핸들러를 버튼에 바인딩
var onClick = function(arg) {
    alert("이동 가능한 타입");
}
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 button이라는 이름의 버튼을 가져옵니다.
var cell = page.getCell("button");
//셀의 이벤트 바인딩
cell.bind("click", onClick);
```

예제 2.&#x20;

```
// 이벤트 핸들러에 사용자 정의 매개변수를 전달해야 합니다.
// 매개변수 정의
var text = "이동 가능한 유형";
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 button이라는 이름의 버튼을 가져옵니다.
var cell = page.getCell("button");
//셀의 이벤트 바인딩
cell.bind("click", text, function (arg) {
    alert(arg.data);
});
```



#### Forguncy 사용 예제

1. 페이지 한 개를 생성하고, 버튼을 생성한 후 왼쪽 위 Cell Name에 button이라고 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-bind01.png" alt=""><figcaption></figcaption></figure>

2\. 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-bind02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하고 버튼을 클릭하면 화면에 지정한 이벤트의 문자열이 화면에 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-bind03.gif)
