# unbindAll 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 메서드 <a href="#unbindall-fang-fa-fang-fa" id="unbindall-fang-fa-fang-fa"></a>

&#x20;  Page.unbindAll(targetPage)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 설명 <a href="#unbindall-fang-fa-miao-shu" id="unbindall-fang-fa-miao-shu"></a>

페이지의 모든 이벤트를 바인딩 해제합니다. 이 메서드는 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) **매개 변수 설명입니다** <a href="#unbindall-fang-fa-can-shu-shuo-ming" id="unbindall-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="163">매개변수 </th><th width="131">형식 </th><th width="137">필수여부</th><th>설명 </th></tr></thead><tbody><tr><td>targetPage</td><td>string</td><td>No</td><td>페이지의 이름입니다. 모든 페이지에 대한 이벤트를 바인딩 해제하는 경우 "*"를 사용합니다. 생략하면 현재 페이지의 이벤트가 바인딩 해제됩니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) **반환값**  <a href="#unbindall-fang-fa-fan-hui-zhi" id="unbindall-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366271/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 예제 <a href="#unbindall-fang-fa-shi-li" id="unbindall-fang-fa-shi-li"></a>

다음 예제 코드에서는 unbindAll 메서드를 통해 페이지의 모든 이벤트에 대한 바인딩을 제거합니다.

```
//page1과 page2의 두 페이지가 있는 경우. 현재 페이지는 1페이지입니다.
var eventHandler = function (arg1, arg2) {
    alert(arg2.pageName);
};
// 바인드 이벤트
Forguncy.Page.bind("Loaded", eventHandler);
 
//현재 페이지에 바인딩된 모든 이벤트 바인딩 해제
Forguncy.Page.unbindAll();
 
//페이지 1의 모든 이벤트 바인딩 해제
Forguncy.Page.unbindAll("페이지1");
 
//모든 전역 이벤트 바인딩 해제
Forguncy.Page.unbindAll("*");
```





#### Forguncy 사용 예제

※참고 : unbind와 unbindall은 실제 사용하는 방법은 동일하며, 페이지 내 Event Handler의 수가 얼마나 많은 가에 따라 선택적으로 사용하실 수 있습니다. 이에 따라 같은 ‘사용 예제’를 사용합니다.

1. 이번 예제에서는 페이지 생성 전에 아래와 같이 2개의 js 파일을 생성합니다.\
   (1) 하나는 이벤트를 페이지 로딩 시점(OnLoad)에 binding 하는 스크립트입니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-unbindall01.png" alt=""><figcaption></figcaption></figure>

(2) 다른 하나는 같은 코드 내용이지만, 이벤트를 binding함과 동시에 unbinding 하는 스크립트입니다. \
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-unbindall02.png" alt=""><figcaption></figcaption></figure>

2\. 페이지를 한 개 생성한 후, “페이지 설정” > “사용자 JavaScript”의 폴더 아이콘을 클릭하여 binding한 스크립트를 먼저 가져옵니다.



<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-unbindall03.png" alt=""><figcaption><p><br></p></figcaption></figure>

프로젝트를 저장하여 실행하면, 아래와 같이 페이지 이름을 출력하는 팝업창이 나타납니다.



<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-unbindall04.png" alt=""><figcaption></figcaption></figure>

3\. 이번엔 unbinding 하는 스크립트를 가져옵니다.

<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-unbindall05.png" alt=""><figcaption></figcaption></figure>

프로젝트를 저장하여 실행하면 팝업창이 나타나지 않고, 해당 페이지가 바로 나타납니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-unbindall06.png)
