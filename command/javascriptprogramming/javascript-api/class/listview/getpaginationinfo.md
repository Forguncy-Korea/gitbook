# getPaginationInfo 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365538/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) 메서드 <a href="#getpaginationinfo-fang-fa-fang-fa" id="getpaginationinfo-fang-fa-fang-fa"></a>

&#x20;  ListView.getPaginationInfo()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365538/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) 설명 <a href="#getpaginationinfo-fang-fa-miao-shu" id="getpaginationinfo-fang-fa-miao-shu"></a>

리스트 페이지 번호 정보를 가져옵니다. 리스트뷰 페이징이 없는 경우 반환 값은 null이 됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365538/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) **매개 변수** <a href="#getpaginationinfo-fang-fa-can-shu-shuo-ming" id="getpaginationinfo-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365538/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) **반환값**  <a href="#getpaginationinfo-fang-fa-fan-hui-zhi" id="getpaginationinfo-fang-fa-fan-hui-zhi"></a>

반환 값은 다음과 같습니다.

```
{
//총 페이지 수
"PageCount":3,
// 현재 페이지 인덱스
"PageIndex":0,
// 페이지당 행 수 표시
"MaxRowCountOfOnePage":10
}
```

리스트에 페이징이 없는 경우 반환 값은 null이 됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365538/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) 예제 <a href="#getpaginationinfo-fang-fa-shi-li" id="getpaginationinfo-fang-fa-shi-li"></a>

다음 예제 코드에서는 getPaginationInfo 메서드를 사용하여 리스트뷰 페이지 번호 정보를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
// 페이지 번호 정보 가져오기
var pagingInfo = listview.getPaginationInfo();
// 경고 상자 팝업, 리스트 페이지 번호 정보 표시
alert(JSON.stringify(pagingInfo, null, " "));
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365538/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) 사용 예제 <a href="#getpaginationinfo-fang-fa-shi-li" id="getpaginationinfo-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365538/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092731000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365538/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092731000\&api=v2)셀 범위를 선택하고 셀 유형을 페이지 탐색 버튼을 설정하고 페이징 리스트뷰 이름을 "리스트뷰1"로  모든 페이지당 행 수를 3개로 설정합니다.

<figure><img src="../../../../../.gitbook/assets/image (1922).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365538/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092731000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1867).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365538/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092731000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 페이지 번호 정보 버튼을 클릭하면 총 페이지 번호, 현재 페이지 번호 인덱스 및 페이지당 행 수를 포함하여 테이블의 페이지 번호 정보를 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (2070).png" alt=""><figcaption></figcaption></figure>
