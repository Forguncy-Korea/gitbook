# getListViews 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366468/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 메서드 <a href="#getlistviews-fang-fa-fang-fa" id="getlistviews-fang-fa-fang-fa"></a>

&#x20;  SubPage.getListViews()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366468/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 설명 <a href="#getlistviews-fang-fa-miao-shu" id="getlistviews-fang-fa-miao-shu"></a>

&#x20;  하위 페이지의 모든 리스트뷰를 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366468/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) **매개 변수**  <a href="#getlistviews-fang-fa-can-shu-shuo-ming" id="getlistviews-fang-fa-can-shu-shuo-ming"></a>

&#x20;  없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366468/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) **반환값**  <a href="#getlistviews-fang-fa-fan-hui-zhi" id="getlistviews-fang-fa-fan-hui-zhi"></a>

[ ListView](../listview/)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366468/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 예제 <a href="#getlistviews-fang-fa-shi-li" id="getlistviews-fang-fa-shi-li"></a>

다음 예제 코드에서는 getListViews 메서드를 사용 하 여 하위 페이지의 모든 리스트뷰 가져오고 반환 된 리스트뷰 인스턴스의 길이를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//페이지 컨테이너 셀 객체 가져오기
var cell = page.getCell("Container");
//페이지 컨테이너의 자식 페이지 가져오기
var subPage = cell.getContentPage();
//서브페이지의 모든 테이블 가져오기
var listview = subPage.getListViews();
//리스트 인스턴스의 길이 가져오기
var len = listview.length;
//리스트뷰 인스턴스의 길이를 보여주는 경고 상자 팝업
alert(len);
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366468/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 사용 예제 <a href="#getlistviews-fang-fa-shi-li" id="getlistviews-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72366468/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092749000\&api=v2)페이지 1에 여러 테이블을 바인딩합니다.

<figure><img src="../../../../../.gitbook/assets/image (1579).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366468/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092748000\&api=v2)  페이지 2에서 셀 범위를 선택하고 셀 유형을 페이지 내 컨텐츠가 포함된 셀로 설정하고 이름을 "Container"로 지정하고 하위 페이지를 페이지 1로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1878).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366468/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092749000\&api=v2)페이지 2에서 셀 범위를 선택하고, 셀 유형을 버튼으로 설정하고, 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고, JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1870).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366468/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092749000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼 클릭하면 가져온 하위 페이지의 모든 테이블 인스턴스 길이를 보여 주는 경고 상자가 나타납니다.<br>

<figure><img src="../../../../../.gitbook/assets/image (1868).png" alt=""><figcaption></figcaption></figure>
