# getListViews 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366059/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 메서드 <a href="#getlistviews-fang-fa-fang-fa" id="getlistviews-fang-fa-fang-fa"></a>

&#x20;  Page.getListViews(includeSubPage)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366059/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 설명 <a href="#getlistviews-fang-fa-miao-shu" id="getlistviews-fang-fa-miao-shu"></a>

페이지의 모든 리스트뷰를 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366059/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) **매개 변수**  <a href="#getlistviews-fang-fa-can-shu-shuo-ming" id="getlistviews-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="164.33333333333331">매개변수 </th><th width="193">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>includeSubPage</td><td>Boolean</td><td>하위 페이지에서 찾을지 여부입니다. 선택적 매개 변수( 기본값은 true)입니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366059/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) **반환값**  <a href="#getlistviews-fang-fa-fan-hui-zhi" id="getlistviews-fang-fa-fan-hui-zhi"></a>

&#x20;     [ListView\[\]](../listview/)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366059/blue%20block.png?version=1\&modificationDate=1648092739000\&api=v2) 예제 <a href="#getlistviews-fang-fa-shi-li" id="getlistviews-fang-fa-shi-li"></a>

다음 예제 코드에서는 getListViews 메서드를 통해 페이지의 모든 리스트뷰 가져옵니다.

```
 //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;

  //페이지 내 ListView 인스턴스들을 불러옵니다.
  var listview = page.getListViews();
  
  //ListView 인스턴스 그룹의 길이를 확인합니다.
  var len = listview.length;
  
  //ListView 인스턴스 그룹의 길이를 화면에 표시합니다.
  alert(len);
```



#### Forguncy 사용 예제

1.  페이지를 한 개 생성하여 Database Table을 연결하는 ListView를 생성합니다.



    <figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getlistviews01.png" alt=""><figcaption></figcaption></figure>
2.  해당 페이지에 버튼을 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령을 추가합니다.<br>

    <figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getlistviews02.png" alt=""><figcaption></figcaption></figure>
3.  프로젝트를 실행하여 버튼을 누르면 getListViews에서 화면의 ListView 개수를 화면에 표시합니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getlistviews03.gif)

<br>
