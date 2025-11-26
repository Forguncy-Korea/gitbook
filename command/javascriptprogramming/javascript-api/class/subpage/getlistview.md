# getListView 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366455/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 메서드 <a href="#getlistview-fang-fa-fang-fa" id="getlistview-fang-fa-fang-fa"></a>

&#x20;  SubPage.getListView(name)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366455/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 설명 <a href="#getlistview-fang-fa-miao-shu" id="getlistview-fang-fa-miao-shu"></a>

리스트뷰 이름으로 하위 페이지의 리스트뷰 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366455/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) **매개 변수** <a href="#getlistview-fang-fa-can-shu-shuo-ming" id="getlistview-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="202.33333333333331">매개변수 </th><th width="210">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>name</td><td>string</td><td>리스트뷰 이름입니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366455/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) **반환값**  <a href="#getlistview-fang-fa-fan-hui-zhi" id="getlistview-fang-fa-fan-hui-zhi"></a>

&#x20;  [ListView](../listview/)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366455/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 예제 <a href="#getlistview-fang-fa-shi-li" id="getlistview-fang-fa-shi-li"></a>

다음 예제 코드에서는 getListView 메서드를 통해 하위 페이지에 지정 된 리스트뷰를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//페이지 컨테이너 셀 객체 가져오기
var cell = page.getCell("Container");
//페이지 컨테이너의 자식 페이지 가져오기
var subPage = cell.getContentPage();
//서브페이지에서 폼 가져오기
var listview = subPage.getListView("리스트뷰1");
// 리스트뷰 이름 가져오기
var name = listview.getName();
// 경고 상자 팝업, 리스트뷰 이름 표시
alert(name);
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366455/blue%20block.png?version=1\&modificationDate=1648092748000\&api=v2) 사용 예제 <a href="#getlistview-fang-fa-shi-li" id="getlistview-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72366455/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092748000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

<figure><img src="../../../../../.gitbook/assets/image (816).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366455/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092748000\&api=v2)페이지 2에서 셀 범위를 선택하고 셀 유형을 페이지 내 컨텐츠가 포함된 셀로 설정하고 이름을 "Container"로 지정하고 하위 페이지를 페이지 1로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1199).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366455/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092748000\&api=v2)페이지 2에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 JavaScript 명령으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1880).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72366455/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092748000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 리스트뷰 이름 가져오기버튼을 클릭하면 반환된 리스트 이름을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1498).png" alt=""><figcaption></figcaption></figure>
