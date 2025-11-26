# getMasterPageName 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366484/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 메서드 <a href="#getmasterpagename-fang-fa-fang-fa" id="getmasterpagename-fang-fa-fang-fa"></a>

&#x20;  SubPage.getMasterPageName()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366484/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 설명 <a href="#getmasterpagename-fang-fa-miao-shu" id="getmasterpagename-fang-fa-miao-shu"></a>

하 페이지의 마스터 페이지 이름을 가져옵니다. 하위페이지에 마스터 페이지가 없는 경우 null을 반환합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366484/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) **매개 변수** <a href="#getmasterpagename-fang-fa-can-shu-shuo-ming" id="getmasterpagename-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366484/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) **반환값**  <a href="#getmasterpagename-fang-fa-fan-hui-zhi" id="getmasterpagename-fang-fa-fan-hui-zhi"></a>

&#x20;  string

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366484/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 예제 <a href="#getmasterpagename-fang-fa-shi-li" id="getmasterpagename-fang-fa-shi-li"></a>

다음 예제 코드에서는 getMasterPageName 메서드를 사용 하 여 하위 페이지의 마스터 페이지 이름을 가져옵니다. 하위 페이지에 마스터 페이지가 없는 경우 null을 반환합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//페이지 컨테이너 셀 객체 가져오기
var cell = page.getCell("Container");
//페이지 컨테이너의 자식 페이지 가져오기
var subPage = cell.getContentPage();
//자식 페이지의 마스터 페이지 이름 가져오기
var masterPageName = subPage.getMasterPageName();
//마스터 페이지의 이름을 보여주는 경고 상자 팝업
alert(masterPageName);
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366484/blue%20block.png?version=1\&modificationDate=1648092749000\&api=v2) 사용 예제 <a href="#getmasterpagename-fang-fa-shi-li" id="getmasterpagename-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72366484/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092749000\&api=v2)페이지 1에서 셀 범위를 선택하고 셀 유형을 페이지 내 컨텐츠가 포함된 셀로 설정하고 이름을 "Container"로 지정하고 하위 페이지를 페이지 2로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1181).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366484/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092749000\&api=v2) 페이지 2를 선택하고 마우스 오른쪽 버튼을 클릭한 다음 오른쪽 클릭 메뉴에서 마스터 페이지 설정을 선택한 다음 목록에서 마스터 페이지를 선택합니다.

<figure><img src="../../../../../.gitbook/assets/image (1466).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366484/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092749000\&api=v2)페이지 1에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 JavaScript 명령으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (780).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366484/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092749000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 클릭하면 하위 페이지의 마스터 페이지 이름을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1177).png" alt=""><figcaption></figcaption></figure>
