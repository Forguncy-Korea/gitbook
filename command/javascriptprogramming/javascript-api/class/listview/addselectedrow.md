# addSelectedRow 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365407/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 메서드 <a href="#addselectedrow-fang-fa-fang-fa" id="addselectedrow-fang-fa-fang-fa"></a>

&#x20;  ListView.addSelectedRow(rowIndex)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365407/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 설명입니다 <a href="#addselectedrow-fang-fa-miao-shu" id="addselectedrow-fang-fa-miao-shu"></a>

리스트뷰에서 지정된 행을 선택합니다. 리스트뷰를 여러 번 선택할 수 있는 경우 행을 선택한 후 이 메서드를 사용하여 지정된 행을 하나 더 선택할 수 있습니다. 리스트뷰에서 라디오만 허용하는 경우 행을 선택한 다음 이 메서드를 사용하여 지정된 행을 선택하고 이전 행은 선택 취소합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365407/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **매개 변수 설명입니다** <a href="#addselectedrow-fang-fa-can-shu-shuo-ming" id="addselectedrow-fang-fa-can-shu-shuo-ming"></a>

| 매개변수     | 형식     | 설명                 |
| -------- | ------ | ------------------ |
| rowIndex | number | 0부터 시작하는 행 인덱스입니다. |

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365407/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **반환값**  <a href="#addselectedrow-fang-fa-fan-hui-zhi" id="addselectedrow-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365407/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 예제 <a href="#addselectedrow-fang-fa-shi-li" id="addselectedrow-fang-fa-shi-li"></a>

다음 예제 코드에서는 addSelectedRow 메서드를 사용하여 리스트뷰에서 지정된 행을 선택합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("리스트1");
//지정된 행 선택
listview.addSelectedRow(2);
```

#### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. 데이터베이스 테이블을 한 개 생성한 후, 이름/생년월일/부서 열을 생성합니다.\
   데이터는 넣어도 되고 안 넣어도 됩니다. 본 예제에서는 알아보기 쉽게 하기 위해 가짜 데이터를 입력했습니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow01.png" alt=""><figcaption></figcaption></figure>

2\. 화면의 영역을 선택하고 “ListView로 설정” 기능을 이용하여, ListView를 생성합니다.\
이 때, 데이터베이스를 선택하라고 나타나는데, 위에서 생성한 테이블을 선택하시면 됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow02.png" alt=""><figcaption></figcaption></figure>

3\. 생성한 ListView의 제일 왼쪽 셀을 클릭 한 뒤, “디자인 탭 > 선택한 열” 옵션을 클릭합니다.\
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addselectedrow05.png" alt=""><figcaption></figcaption></figure>

4\. ListView에 데이터를 쉽게 입력하는 방법은 아래와 같습니다. 테이블의 열-이름을 드래그하면 됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addselectedrow06.gif" alt=""><figcaption></figcaption></figure>

5\. 버튼을 한 개 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령을 이용하여 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addselectedrow07.png" alt=""><figcaption></figcaption></figure>

6\. 프로젝트를 생성합니다. 버튼을 클릭하면 ListView의 세 번 째 줄의 체크 박스가 선택됩니다.

\
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addselectedrow08.gif" alt=""><figcaption></figcaption></figure>

참고 : ListView의 Index는 0에서부터 시작합니다. 첫 번 째 데이터부터 0, 1, 2, 3, … 순으로 늘어납니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addselectedrow09.png)

<br>
