# getText 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365612/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 메서드 <a href="#gettext-fang-fa-fang-fa" id="gettext-fang-fa-fang-fa"></a>

&#x20;  ListView.getText(rowIndex, column)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365612/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 설명 <a href="#gettext-fang-fa-miao-shu" id="gettext-fang-fa-miao-shu"></a>

리스트뷰의 지정된 셀에 있는 텍스트를 가져옵니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365612/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) **매개 변수 설명입니다** <a href="#gettext-fang-fa-can-shu-shuo-ming" id="gettext-fang-fa-can-shu-shuo-ming"></a>

| 매개변수     | 유형               | 설명                                         |
| -------- | ---------------- | ------------------------------------------ |
| rowIndex | number           | 0부터 시작하는 테이블의 행 인덱스입니다.                    |
| column   | string 또는 number | 테이블의 열 이름 또는 열 인덱스의 숫자로, 열 인덱스는 0부터 시작합니다. |

#### &#x20;![](https://help.grapecity.com.cn/download/thumbnails/72365612/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) **반환값**  <a href="#gettext-fang-fa-fan-hui-zhi" id="gettext-fang-fa-fan-hui-zhi"></a>

&#x20;  any

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365612/blue%20block.png?version=1\&modificationDate=1648092732000\&api=v2) 예제 <a href="#gettext-fang-fa-shi-li" id="gettext-fang-fa-shi-li"></a>

다음 예제 코드에서 getText 메서드를 사용 하 여  리스트뷰 지정 셀의 텍스트를 가져옵니다.

리스트뷰의 네 번째 열의 열 이름은 부서이며 부서 열의 첫 번째 행 셀에 있는 텍스트를 가져옵니다.

예1.&#x20;

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트1");
//리스트뷰의 지정된 셀에 있는 텍스트를 가져옵니다.
var text = listview.getText(0,"부서");
//지정된 셀에 텍스트를 표시하기 위해 경고 상자를 표시합니다.
alert(text);
```

예2.&#x20;

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트1");
// 리스트의 지정된 셀에 있는 텍스트를 가져옵니다.
var text = listview.getText(0,3);
// 지정된 셀에 텍스트를 표시하기 위해 경고 상자를 표시합니다.
alert(text);
```

![](https://help.grapecity.com.cn/download/thumbnails/72365612/16.png?version=1\&modificationDate=1648092732000\&api=v2)**사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365612/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092732000\&api=v2)페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 각 열의 열 이름을 설정합니다.

테이블이 켜져 있으면 편집할 수 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365612/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092732000\&api=v2)테이블에서 부서 열을 선택하고 셀 유형을 콤보 상자로 설정하고 데이터베이스에서 프로젝트를 생성합니다.

<figure><img src="../../../../../.gitbook/assets/image (1290).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365612/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092732000\&api=v2)셀 범위를 선택하고 셀 유형을 버튼 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1366).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365612/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092732000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 테이블의 부서 열에서 편집 상태를 입력한 후 목록에서 부서를 선택한 다음 텍스트 가져오기 버튼을 클릭하면 표의 지정된 셀에 있는 텍스트가 표시됩니다.

<figure><img src="../../../../../.gitbook/assets/image (774).png" alt=""><figcaption></figcaption></figure>
