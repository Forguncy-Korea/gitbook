# addNewRow 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365390/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 메서드 <a href="#addnewrow-fang-fa-fang-fa" id="addnewrow-fang-fa-fang-fa"></a>

&#x20;  ListView.addNewRow(rowValues, isText)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365390/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 설명 <a href="#addnewrow-fang-fa-miao-shu" id="addnewrow-fang-fa-miao-shu"></a>

리스트뷰에 새 행에 대한 데이터를 포함하여 새 행을 추가합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365390/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **매개 변수 설명입니다** <a href="#addnewrow-fang-fa-can-shu-shuo-ming" id="addnewrow-fang-fa-can-shu-shuo-ming"></a>

| 매개 변수     | 형식                    | 설명                                                         |
| --------- | --------------------- | ---------------------------------------------------------- |
| rowValues | plainObject 또는 any\[] | 새 행의 데이터입니다.                                               |
| isText    | boolean               | 선택적 매개 변수, rowValues의 데이터를 텍스트로 구문 분석할지 여부, 기본값은 false입니다. |

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365390/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **반환값**  <a href="#addnewrow-fang-fa-fan-hui-zhi" id="addnewrow-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365390/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 예제 <a href="#addnewrow-fang-fa-shi-li" id="addnewrow-fang-fa-shi-li"></a>

다음 예제 코드에서는 addNewRow 메서드를 통해 테이블에 새 행과 데이터 행을 추가합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("리스트뷰1");
//새 줄 추가
listview.addNewRow(
{
"이름": "리 레이",
"생년월일": new Date(1990, 1, 3),
"부서": "마케팅 부서"
});
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365390/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 사용 예제 <a href="#addnewrow-fang-fa-shi-li" id="addnewrow-fang-fa-shi-li"></a>



#### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. 데이터베이스 테이블을 한 개 생성한 후, 이름/생년월일/부서 열을 생성합니다.\
   데이터는 넣어도 되고 안 넣어도 됩니다. 본 예제에서는 알아보기 쉽게 하기 위해 가짜 데이터를 입력했습니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow01.png" alt=""><figcaption></figcaption></figure>

2\. 화면의 영역을 선택하고 “ListView로 설정” 기능을 이용하여, ListView를 생성합니다.\
이 때, 데이터베이스를 선택하라고 나타나는데, 위에서 생성한 테이블을 선택하시면 됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow02.png" alt=""><figcaption></figcaption></figure>

3\. ListView에 데이터를 쉽게 입력하는 방법은 아래와 같습니다. 테이블의 열-이름을 드래그하면 됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow03.gif" alt=""><figcaption></figcaption></figure>

4\. ListView의 이름을 설정합니다. ListView의 이름은 클릭 시 오른쪽의 ‘셀 유형’ 탭에서 나타납니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow04.png" alt=""><figcaption></figcaption></figure>

5\. ListView 내부의 각 열-이름을 설정합니다. ListView의 2번 째 줄에 열 이름을 정할 수 있습니다.\
이렇게 설정해야 ListView라는 형식의 control을 웹에서 사용할 수 있습니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow05.png" alt=""><figcaption></figcaption></figure>

6\. 버튼을 한 개 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령을 이용하여 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow06.png" alt=""><figcaption></figcaption></figure>

7\. 프로젝트를 생성합니다. 버튼을 클릭하면 ListView에 데이터가 입력됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-addnewrow07.gif)
