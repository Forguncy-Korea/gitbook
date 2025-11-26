# getPageName 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366503/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 메서드 <a href="#getpagename-fang-fa-fang-fa" id="getpagename-fang-fa-fang-fa"></a>

SubPage.getPageName()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366503/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 설명 <a href="#getpagename-fang-fa-miao-shu" id="getpagename-fang-fa-miao-shu"></a>

하위 페이지의 이름을 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366503/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) **매개 변수** <a href="#getpagename-fang-fa-can-shu-shuo-ming" id="getpagename-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366503/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) **반환값**  <a href="#getpagename-fang-fa-fan-hui-zhi" id="getpagename-fang-fa-fan-hui-zhi"></a>

&#x20; string&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366503/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 예제 <a href="#getpagename-fang-fa-shi-li" id="getpagename-fang-fa-shi-li"></a>

다음 예제 코드에서 getPageName 메서드를 사용 하 여 하위 페이지의 이름을 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//페이지 컨테이너 셀 객체 가져오기
var cell = page.getCell("Container");
//페이지 컨테이너의 자식 페이지 가져오기
var subpage = cell.getContentPage();
//하위 페이지의 이름을 가져옵니다.
var pageName = subpage .getPageName();
// 경고 상자 팝업, 하위 페이지 이름 표시
alert(pageName);
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366503/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 사용 예제 <a href="#getpagename-fang-fa-shi-li" id="getpagename-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72366484/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092749000\&api=v2)페이지 1에서 셀 범위를 선택하고 셀 유형을 페이지 내 컨텐츠가 포함된 셀로 설정하고 이름을 "Container"로 지정하고 하위 페이지를 페이지 2로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (646).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366503/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092749000\&api=v2) 페이지 1에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1779).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366503/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092749000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 클릭하면 하위 페이지의 이름을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (595).png" alt=""><figcaption></figcaption></figure>
