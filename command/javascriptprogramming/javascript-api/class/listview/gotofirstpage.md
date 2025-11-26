# goToFirstPage 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365640/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 메서드 <a href="#gotofirstpage-fang-fa-fang-fa" id="gotofirstpage-fang-fa-fang-fa"></a>

&#x20;  ListView.goToFirstPage()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365640/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 설명 <a href="#gotofirstpage-fang-fa-miao-shu" id="gotofirstpage-fang-fa-miao-shu"></a>

리스트뷰 페이지 매김 탐색 버튼을 사용하여 리스트 데이터를 페이징하는 경우 이 방법을 사용하면 리스트뷰 첫 번째 페이지로 이동하여 첫 번째 페이지의 데이터를 표시할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365640/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) **매개 변수** <a href="#gotofirstpage-fang-fa-can-shu-shuo-ming" id="gotofirstpage-fang-fa-can-shu-shuo-ming"></a>

**없음**&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365640/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) **반환값**  <a href="#gotofirstpage-fang-fa-fan-hui-zhi" id="gotofirstpage-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365640/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 예제입니다 <a href="#gotofirstpage-fang-fa-shi-li" id="gotofirstpage-fang-fa-shi-li"></a>

다음 예제 코드에서는 goToFirstPage 메서드를 통해 표시되는 리스트 데이터가 첫 페이지로 이동합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
//리스트의 첫 페이지로 이동
listview.goToFirstPage()
```

\
![](https://help.grapecity.com.cn/download/thumbnails/72365640/16.png?version=1\&modificationDate=1648092732000\&api=v2)**절차를 따르십시오**

![](https://help.grapecity.com.cn/download/thumbnails/72365640/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092732000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365640/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092732000\&api=v2)셀 범위를 선택하고 셀 유형을 페이지 탐색 버튼로 설정하고  페이징 리스트뷰 이름을 리스트뷰로설정하고 페이지당 행 수를 3개로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1023).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365725/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092734000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (969).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365640/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092732000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고, 페이지를 뒤집고, 두 번째 페이지를 표시하고, 첫 번째 페이지 단추를 클릭하면 첫 번째 페이지로 돌아갑니다.

<figure><img src="../../../../../.gitbook/assets/image (1242).png" alt=""><figcaption></figcaption></figure>
