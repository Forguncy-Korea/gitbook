# bind 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365984/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 메서드 <a href="#bind-fang-fa-fang-fa" id="bind-fang-fa-fang-fa"></a>

&#x20;  Page.bind(type, data, fn, targetPage)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365984/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 설명 <a href="#bind-fang-fa-miao-shu" id="bind-fang-fa-miao-shu"></a>

&#x20;  페이지에 이벤트를 바인딩합니다. 현재 페이지, 지정된 페이지 또는 모든 페이지에 이벤트를 바인딩할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365984/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) **매개 변수** <a href="#bind-fang-fa-can-shu-shuo-ming" id="bind-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="147">매개변수 </th><th width="116">형식 </th><th width="130">필수여부 </th><th>설명 </th></tr></thead><tbody><tr><td>eventType</td><td>string</td><td>YES</td><td>페이지 이벤트 유형을 나타내는 문자열입니다. 페이지에서 지원되는 이벤트는 <a href="../pageevents/">PageEvents 클래스</a> 를 참조하십시오.</td></tr><tr><td>data</td><td>any</td><td>NO</td><td>이벤트 처리기에 전달된 사용자 지정 매개 변수를 무시하지 않는 경우 선택적 매개 변수입니다.</td></tr><tr><td>fn</td><td>function</td><td>YES</td><td>이벤트 처리기입니다. 이벤트에는 arg1, arg2의 두 가지 매개 변수가 있습니다. arg1 매개 변수는 data 매개 변수를 나타내고 arg2는 targetPage 매개 변수를 나타냅니다.</td></tr><tr><td>targetPage</td><td>string</td><td>NO</td><td>페이지의 이름입니다. 모든 페이지에 대한 이벤트를 바인딩하는 경우 "*"를 사용합니다. 생략하면 현재 페이지에 바인딩됩니다.</td></tr></tbody></table>

#### &#x20;![](https://help.grapecity.com.cn/download/thumbnails/72365984/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) **반환값**  <a href="#bind-fang-fa-fan-hui-zhi" id="bind-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365984/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 예제 <a href="#bind-fang-fa-shi-li" id="bind-fang-fa-shi-li"></a>

다음 예제 코드에서는 bnd 메서드를 통해 페이지에 이벤트를 바인딩합니다.

**예 1:**

이벤트 처리기에는 사용자 지정 매개 변수를 전달할 필요가 없으며 이벤트가 현재 페이지에 바인딩됩니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//바인드 페이지 이벤트
page.bind("loaded", function (arg1, arg2) {
//페이지의 페이지 이름을 보여주는 경고 상자가 나타납니다.
alert(arg2.pageName);
});
```

**예 2:**

이벤트 처리기에는 사용자 지정 매개 변수를 전달하고 이벤트는 페이지 1에 바인딩해야 합니다.

```
//맞춤 매개변수
var text = "ready";
// 현재 페이지 가져오기
var page = Forguncy.Page;
//바인드 페이지 이벤트
page.bind("loaded", text, function (arg1, arg2) {
//사용자 정의 매개변수의 내용을 표시하기 위해 경고 상자가 나타납니다.
alert(arg1.data);
}, "페이지 1");
```

**예 3:**

이벤트 처리기에는 사용자 지정 매개 변수를 전달하고 이벤트를 모든 페이지에 바인딩해야 합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//바인드 페이지 이벤트
page.bind("loaded", function (arg1, arg2) {
//페이지로 이동시 프롬프트박스의 내용은 1페이지, 2페이지로 이동시 프롬프트박스의 내용은 2페이지
alert(arg2.pageName);
}, "*");
```

#### Forguncy 사용 예제

1. 페이지가 로딩되는 시점에 팝업 메시지를 띄우는 예제를 JavaScript로 생성하여, Forguncy의 특정 페이지(예제에서는 ‘페이지1’이라는 이름의 페이지)에 불러옵니다. ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-bind-01.png)\
   <br>
2. 해당 프로젝트를 실행하면 페이지가 표시되기 전에 해당 Forguncy 페이지의 이름인 ‘페이지1’이 팝업으로 표시됩니다. 팝업에서 ‘확인’을 누르면 이후 페이지 내용이 표시됩니다. ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-bind-02.gif)

<br>
