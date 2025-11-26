# Loaded 이벤트

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365923/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 이벤트 <a href="#loaded-shi-jian-shi-jian" id="loaded-shi-jian-shi-jian"></a>

&#x20;  Forguncy.PageEvents.Loaded

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365923/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 설명 <a href="#loaded-shi-jian-miao-shu" id="loaded-shi-jian-miao-shu"></a>

페이지가 로드된 후 이벤트가 트리거됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365923/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) **반환값**  <a href="#loaded-shi-jian-fan-hui-zhi" id="loaded-shi-jian-fan-hui-zhi"></a>

문자열

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365923/blue%20block.png?version=1\&modificationDate=1648092738000\&api=v2) 예제 <a href="#loaded-shi-jian-shi-li" id="loaded-shi-jian-shi-li"></a>

다음 예제 코드에서는 bnd 메서드를 통해 페이지에 Loaded 이벤트를 추가하고 페이지가 로드될 때 경고 상자가 나타납니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//페이지 Loaded 이벤트 바인딩
page.bind("loaded", function (arg1, arg2) {
//페이지 이름을 보여주는 팝업창이 나타납니다.
alert(arg2.pageName);
});
```

![](https://help.grapecity.com.cn/download/thumbnails/72365923/16.png?version=1\&modificationDate=1648092738000\&api=v2)**사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365923/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092738000\&api=v2)페이지 설정에서 JavaScript 파일을 업로드하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1701).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365923/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092738000\&api=v2)페이지를 실행하면 페이지가 로드될 때 페이지 1의 페이지 이름을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (672).png" alt=""><figcaption></figcaption></figure>
