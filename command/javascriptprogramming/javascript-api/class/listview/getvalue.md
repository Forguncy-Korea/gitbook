# getValue 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365628/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 메서드 <a href="#getvalue-fang-fa-fang-fa" id="getvalue-fang-fa-fang-fa"></a>

&#x20;  ListView.getValue(rowIndex, column)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365628/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 설명 <a href="#getvalue-fang-fa-miao-shu" id="getvalue-fang-fa-miao-shu"></a>

리스트의 지정된 위치에 있는 셀의 값을 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365628/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) **매개 변수**  <a href="#getvalue-fang-fa-can-shu-shuo-ming" id="getvalue-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="201.33333333333331">매개변수 </th><th width="174">유형 </th><th>설명 </th></tr></thead><tbody><tr><td>rowIndex</td><td>number</td><td>리스트뷰의 행 인덱스입니다. 행 인덱스는 0부터 시작합니다.</td></tr><tr><td>column</td><td>string 또는 number</td><td>리스트뷰의 열 이름 또는 열 인덱스는 0부터 시작합니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365628/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) **값을 반환합니다** <a href="#getvalue-fang-fa-fan-hui-zhi" id="getvalue-fang-fa-fan-hui-zhi"></a>

&#x20;  any

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365628/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 예제입니다 <a href="#getvalue-fang-fa-shi-li" id="getvalue-fang-fa-shi-li"></a>

다음 예제 코드에서는 getValue 메서드를 사용 하 여 리스트뷰의 지정 된 위치에 셀의 값을 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
// 리스트의 지정된 위치에 있는 셀의 값을 가져오기 위해 경고 상자를 표시합니다.
alert(listview.getValue(0,"이름"));
```

\
![](https://help.grapecity.com.cn/download/thumbnails/72365628/16.png?version=1\&modificationDate=1648092732000\&api=v2)**사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365628/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092732000\&api=v2)페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 각 열의 열 이름을 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365628/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092732000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1024).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365628/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092732000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 셀 값 가져오기 버튼을 클릭하면 표의 지정된 위치에 있는 셀의 값을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1025).png" alt=""><figcaption></figcaption></figure>
