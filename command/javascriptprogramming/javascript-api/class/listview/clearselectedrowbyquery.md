# clearSelectedRowByQuery 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365450/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 메서드 <a href="#clearselectedrowbyquery-fang-fa-fang-fa" id="clearselectedrowbyquery-fang-fa-fang-fa"></a>

&#x20;  ListView.clearSelectedRowByQuery()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365450/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 설명 <a href="#clearselectedrowbyquery-fang-fa-miao-shu" id="clearselectedrowbyquery-fang-fa-miao-shu"></a>

쿼리 조건에 따라 리스트의 선택 행을 지웁니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365450/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **매개 변수**  <a href="#clearselectedrowbyquery-fang-fa-can-shu-shuo-ming" id="clearselectedrowbyquery-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="183.33333333333331">매개변수 </th><th width="181">형식 </th><th>설명 </th></tr></thead><tbody><tr><td> query</td><td> object</td><td>기본 키 이름을 기본 키로 사용하여 해당 데이터를 값으로 사용하여 선택한 행에 대한 쿼리 조건입니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365450/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **반환값**  <a href="#clearselectedrowbyquery-fang-fa-fan-hui-zhi" id="clearselectedrowbyquery-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365450/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 예제 <a href="#clearselectedrowbyquery-fang-fa-shi-li" id="clearselectedrowbyquery-fang-fa-shi-li"></a>

다음 예제 코드에서는 clearSelectedRowByQuery 메서드를 사용하여 쿼리 조건에 따라 리스트의 선택 행을 지웁니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
//// 쿼리 조건에 따라 리스트의 선택된 행을 지웁니다.
listview.clearSelectedRowByQuery({ID:1});
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365450/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 사용 예제 <a href="#clearselectedrowbyquery-fang-fa-shi-li" id="clearselectedrowbyquery-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365450/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092729000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365450/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092729000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (781).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365450/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092729000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 테이블에서 데이터 행을 선택한 다음 행 선택 지우기 버튼 누르면 쿼리 조건에 따라 테이블의 선택 행이 지워집니다.

<figure><img src="../../../../../.gitbook/assets/image (1226).png" alt=""><figcaption></figcaption></figure>
