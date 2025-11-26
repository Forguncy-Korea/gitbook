# setText 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365780/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) 메서드 <a href="#settext-fang-fa-fang-fa" id="settext-fang-fa-fang-fa"></a>

&#x20;  ListView.setText(rowIndex: number, column: string | number, text: any)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365780/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) 설명 <a href="#settext-fang-fa-miao-shu" id="settext-fang-fa-miao-shu"></a>

리스트뷰의 지정된 위치에 있는 셀의 텍스트를 설정합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365780/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) **매개 변수 설명입니다** <a href="#settext-fang-fa-can-shu-shuo-ming" id="settext-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="172.33333333333331">매개변수 </th><th width="199">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>rowIndex</td><td>number</td><td>0부터 시작하는 테이블의 행 인덱스입니다.</td></tr><tr><td>column</td><td>string 또는 number</td><td>테이블의 열 이름 또는 열 인덱스의 숫자로, 열 인덱스는 0부터 시작합니다.</td></tr><tr><td>text</td><td>any</td><td>설정된 텍스트입니다.</td></tr></tbody></table>

#### &#x20;![](https://help.grapecity.com.cn/download/thumbnails/72365780/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) **반환값**  <a href="#settext-fang-fa-fan-hui-zhi" id="settext-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365780/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) 예제 <a href="#settext-fang-fa-shi-li" id="settext-fang-fa-shi-li"></a>

다음 예제 코드에서는 setText 메서드를 사용 하 여 리스트뷰의 위치를 지정 하는 셀에 대 한 텍스트를 설정 합니다.

**예 1:**

리스트뷰의 첫 번째 열의 열 이름은 이름이며 세 번째 행 이름 열의 셀에 대한 텍스트는 "리시"로 설정됩니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
// 리스트의 지정된 위치에 있는 셀에 텍스트를 설정합니다.
listview.setText(2,"이름","리시");
```

**예 2:**

리스트뷰의 이름은 첫 번째 열로 나열되고 세 번째 행의 두 번째 열에 있는 셀의 텍스트는 리로 설정됩니다.

```
// 현재 페이지 가져오기
var 페이지 = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("리스트 ");
// 테이블의 지정된 위치에 있는 셀에 텍스트를 설정합니다.
listview.setText(2,1,"리시");
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365780/blue%20block.png?version=1\&modificationDate=1648092735000\&api=v2) 사용 예제 <a href="#settext-fang-fa-shi-li" id="settext-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365780/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092735000\&api=v2)페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 각 열의 열 이름을 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365725/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092734000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (734).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365780/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092735000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 텍스트 설정 버튼 클릭하면 표의 위치를 지정하는 셀에 텍스트가 설정됩니다.

<figure><img src="../../../../../.gitbook/assets/image (1340).png" alt=""><figcaption></figcaption></figure>
