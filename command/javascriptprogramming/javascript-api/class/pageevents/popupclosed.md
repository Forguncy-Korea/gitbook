# PopupClosed 이벤트

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365955/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 이벤트 <a href="#popupclosed-shi-jian-shi-jian" id="popupclosed-shi-jian-shi-jian"></a>

&#x20;  Forguncy.PageEvents.PopupClosed

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365955/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 설명 <a href="#popupclosed-shi-jian-miao-shu" id="popupclosed-shi-jian-miao-shu"></a>

이 이벤트는 현재 페이지의 팝업 페이지가 닫힐 때 트리거됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365955/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) **반환값**  <a href="#popupclosed-shi-jian-fan-hui-zhi" id="popupclosed-shi-jian-fan-hui-zhi"></a>

문자열

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365955/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 예제 <a href="#popupclosed-shi-jian-shi-li" id="popupclosed-shi-jian-shi-li"></a>

다음 예제 코드에서는 bnd 메서드를 통해 페이지에 PopupClosed 이벤트를 추가하고 현재 페이지의 팝업 페이지를 닫을 때 경고 상자가 나타납니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//바인드 페이지 이벤트
page.bind("popupClosed", function () {
/// 경고 상자 팝업
alert("이동 가능한 타입");
});
```

![](https://help.grapecity.com.cn/download/thumbnails/72365955/16.png?version=1\&modificationDate=1648092738000\&api=v2)사용 예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365955/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092738000\&api=v2)페이지 설정에서 JavaScript 파일을 업로드하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1610).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365955/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092738000\&api=v2)페이지를 실행하고 테이블에서 팝업버튼을 클릭하여 팝업페이지를 띄우고, 닫기 버튼을 클릭하여 팝업 페이지가 닫히면 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1873).png" alt=""><figcaption></figcaption></figure>
