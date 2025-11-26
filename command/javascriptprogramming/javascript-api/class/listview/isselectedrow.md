# isSelectedRow 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365725/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 메서드 <a href="#isselectedrow-fang-fa-fang-fa" id="isselectedrow-fang-fa-fang-fa"></a>

&#x20;  ListView.isSelectedRow(rowIndex)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365725/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 설명 <a href="#isselectedrow-fang-fa-miao-shu" id="isselectedrow-fang-fa-miao-shu"></a>

지정된 행이 선택되었는지 여부를 가져옵니다. 반환 값은 true 또는 false입니다. true는 선택되고 false는 선택되지 않습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365725/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) **매개 변수**  <a href="#isselectedrow-fang-fa-can-shu-shuo-ming" id="isselectedrow-fang-fa-can-shu-shuo-ming"></a>

| 매개변수     | 형식     | 설명                 |
| -------- | ------ | ------------------ |
| rowIndex | number | 0부터 시작하는 행 인덱스입니다. |

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365725/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) **반환값**  <a href="#isselectedrow-fang-fa-fan-hui-zhi" id="isselectedrow-fang-fa-fan-hui-zhi"></a>

&#x20;  boolean

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365725/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 예제 <a href="#isselectedrow-fang-fa-shi-li" id="isselectedrow-fang-fa-shi-li"></a>

다음 예제 코드에서는 isSelectedRow 메서드를 통해 지정된 행이 선택되었는지 여부를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트뷰 가져오기
var listview = page.getListView("리스트뷰 1");
//지정된 행이 선택되었는지 여부를 가져옵니다.
var row = listview.isSelectedRow(2);
// 지정된 행이 선택되었는지 여부를 표시하는 경고 상자 팝업
alert(row);
```

\
![](https://help.grapecity.com.cn/download/thumbnails/72365725/16.png?version=1\&modificationDate=1648092734000\&api=v2)사용 예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365725/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092734000\&api=v2)페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365725/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092734000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1620).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365725/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092734000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 단추를 클릭하면 지정된 행이 선택되었는지 여부를 나타내는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (782).png" alt=""><figcaption></figcaption></figure>
