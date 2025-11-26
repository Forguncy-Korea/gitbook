# getQuery 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365552/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) 메서드입니다 <a href="#getquery-fang-fa-fang-fa" id="getquery-fang-fa-fang-fa"></a>

&#x20;  ListView.getQuery(rowIndex)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365552/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) 설명 <a href="#getquery-fang-fa-miao-shu" id="getquery-fang-fa-miao-shu"></a>

지정된 행의 기본 키를 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365552/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) **매개 변수**  <a href="#getquery-fang-fa-can-shu-shuo-ming" id="getquery-fang-fa-can-shu-shuo-ming"></a>

| 매개 변수    | 형식     | 설명               |
| -------- | ------ | ---------------- |
| rowIndex | number | 행의 행 인덱스를 지정합니다. |

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365552/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) **반환 값**  <a href="#getquery-fang-fa-fan-hui-zhi" id="getquery-fang-fa-fan-hui-zhi"></a>

&#x20;  object

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365552/blue%20block.png?version=1\&modificationDate=1648092731000\&api=v2) 예제 <a href="#getquery-fang-fa-shi-li" id="getquery-fang-fa-shi-li"></a>

다음 예제 코드에서는 getQuery 메서드를 사용 하 여 리스트뷰 지정 행의 기본 키를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
//지정된 행의 기본 키 가져오기
var query = listview.getQuery(0);
//기본 키 정보를 보여주는 경고 상자 팝업
alert(JSON.stringify(query, null, " "));
```

&#x20;\
![](https://help.grapecity.com.cn/download/thumbnails/72365552/16.png?version=1\&modificationDate=1648092731000\&api=v2)**사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365552/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092731000\&api=v2) 페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365552/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092731000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1720).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365552/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092731000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 기본 키 가져오기 버튼을 클릭하면 지정된 행의 기본 키 정보를 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (683).png" alt=""><figcaption></figcaption></figure>
