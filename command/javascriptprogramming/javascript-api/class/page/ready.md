# ready 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366157/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 메서드 <a href="#ready-fang-fa-fang-fa" id="ready-fang-fa-fang-fa"></a>

&#x20;  Page.ready(fn)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366157/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 설명 <a href="#ready-fang-fa-miao-shu" id="ready-fang-fa-miao-shu"></a>

페이지가 준비되면 매개 변수의 콜백 함수가 호출되고 페이지의 처리 논리가 콜백 함수에 기록되어 페이지를 조작할 준비가 되었는지 확인하는 것이 좋습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366157/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) **매개 변수** <a href="#ready-fang-fa-can-shu-shuo-ming" id="ready-fang-fa-can-shu-shuo-ming"></a>

| 매개변수  | 형식       | 설명                                  |
| ----- | -------- | ----------------------------------- |
| fn    | function | 페이지가 완료될 준비가 되면 자동으로 호출되는 콜백 함수입니다. |

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366157/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) **반환값**  <a href="#ready-fang-fa-fan-hui-zhi" id="ready-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366157/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 예제 <a href="#ready-fang-fa-shi-li" id="ready-fang-fa-shi-li"></a>

다음 예제 코드에서는 ready 메서드를 사용하여 ready 메서드의 콜백 함수에 페이지 처리 논리를 추가하여 현재 로그온한 사용자의 사용자 이름을 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//ready 메소드의 콜백 함수에 페이지 처리 로직 추가
page.ready(function () {
//셀 버튼의 이벤트 바인딩
page.getCell("button").bind("click", function () {
//현재 로그인한 사용자의 사용자 이름을 보여주는 경고 상자가 나타납니다.
alert(page.getUserName());
})
});
```

#### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, 셀 범위를 선택하여 “현재 사용자” 셀 유형을 추가합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-ready01.png" alt=""><figcaption></figcaption></figure>

2\. 버튼을 추가합니다. (✅중요) 이 때, 화면 좌측 상단에 Forguncy Cell Name을 ‘button’으로 지정해 줍니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-ready02.png" alt=""><figcaption></figcaption></figure>

3\. ready Method는 페이지의 실행 시점(OnLoad 시점)에 실행되는 스크립트이므로, 외부 파일로 만들어 해당 페이지에 연결해 줍니다.\
아래 그림은 Notepad++로 스크립트를 작성 > 저장 > Forguncy에 가져오기 한 예제입니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-ready03.png" alt=""><figcaption></figcaption></figure>

4\. 해당 프로젝트를 실행하여 버튼을 클릭하면 아래와 같이 현재 사용자의 이름이 나타납니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-ready04.gif)

<br>
