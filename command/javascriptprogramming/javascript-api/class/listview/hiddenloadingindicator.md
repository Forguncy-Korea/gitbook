# hiddenLoadingIndicator 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365712/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 메서드 <a href="#hiddenloadingindicator-fang-fa-fang-fa" id="hiddenloadingindicator-fang-fa-fang-fa"></a>

&#x20;  ListView.hiddenLoadingIndicator()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365712/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 설명 <a href="#hiddenloadingindicator-fang-fa-miao-shu" id="hiddenloadingindicator-fang-fa-miao-shu"></a>

&#x20;  리스트의 로드 아이콘을 숨기고 리스트의 정상적인 사용을 복원합니다. 일반적으로 showLoadingIndicator 메서드와 함께 사용됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365712/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) **매개 변수** <a href="#hiddenloadingindicator-fang-fa-can-shu-shuo-ming" id="hiddenloadingindicator-fang-fa-can-shu-shuo-ming"></a>

&#x20;  없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365712/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) **반환값**  <a href="#hiddenloadingindicator-fang-fa-fan-hui-zhi" id="hiddenloadingindicator-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365712/blue%20block.png?version=1\&modificationDate=1648092733000\&api=v2) 예제 <a href="#hiddenloadingindicator-fang-fa-shi-li" id="hiddenloadingindicator-fang-fa-shi-li"></a>

다음 예제 코드에서는 hiddenLoadingIndicator 메서드를 통해 리스트 로드 아이콘을 숨깁니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("리스트뷰1");
//리스트 로딩 아이콘 숨기기
listview.hiddenLoadingIndicator();
```

![](https://help.grapecity.com.cn/download/thumbnails/72365712/16.png?version=1\&modificationDate=1648092733000\&api=v2)**절차를 따르십시오**

![](https://help.grapecity.com.cn/download/thumbnails/72365712/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092733000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365712/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092733000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍 하]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1270).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365712/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092733000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

* 페이지를 실행하고 페이지에서 로드 표시 아이콘 버튼을 클릭하면 테이블이 로드될 때 아이콘이 표시됩니다.

<figure><img src="../../../../../.gitbook/assets/image (1174).png" alt=""><figcaption></figcaption></figure>



* 로드 숨기기 아이콘을 클릭하면 테이블 로드 아이콘이 숨겨집니다.

<figure><img src="../../../../../.gitbook/assets/image (1333).png" alt=""><figcaption></figcaption></figure>
