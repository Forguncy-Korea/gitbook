# showLoadingIndicator 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365809/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) 메서드 <a href="#showloadingindicator-fang-fa-fang-fa" id="showloadingindicator-fang-fa-fang-fa"></a>

&#x20;  ListView.showLoadingIndicator()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365809/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) 설명 <a href="#showloadingindicator-fang-fa-miao-shu" id="showloadingindicator-fang-fa-miao-shu"></a>

&#x20;  리스트뷰 로드 아이콘을 표시하고 [hiddenLoadingIndicator](https://help.grapecity.com.cn/pages/viewpage.action?pageId=72365712)가 호출될 때까지 리스트뷰를 비활성화합니다. 일반적으로 예기치 않은 작업을 방지하기 위해 리스트뷰를 조작하기 전에 많은 작업을 수행하는 데 사용됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365809/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) **매개 변수** <a href="#showloadingindicator-fang-fa-can-shu-shuo-ming" id="showloadingindicator-fang-fa-can-shu-shuo-ming"></a>

&#x20;  없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365809/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) **반환값**  <a href="#showloadingindicator-fang-fa-fan-hui-zhi" id="showloadingindicator-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365809/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) 예제 <a href="#showloadingindicator-fang-fa-shi-li" id="showloadingindicator-fang-fa-shi-li"></a>

다음 예제 코드에서는 showLoadingIndicator 메서드를 통해 리스트뷰 로드 아이콘을 표시합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
//리스트 로딩 아이콘 표시
 listview.showLoadingIndicator();
```

![](https://help.grapecity.com.cn/download/thumbnails/72365712/16.png?version=1\&modificationDate=1648092733000\&api=v2)**절차를 따르십시오**

![](https://help.grapecity.com.cn/download/thumbnails/72365712/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092733000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365712/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092733000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍 하]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1398).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365712/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092733000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

* 페이지를 실행하고 페이지에서 로드 표시 아이콘 버튼을 클릭하면 테이블이 로드될 때 아이콘이 표시됩니다.

<figure><img src="../../../../../.gitbook/assets/image (1174).png" alt=""><figcaption></figcaption></figure>



* 로드 숨기기 아이콘을 클릭하면 테이블 로드 아이콘이 숨겨집니다.

<figure><img src="../../../../../.gitbook/assets/image (1333).png" alt=""><figcaption></figcaption></figure>
