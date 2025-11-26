# reload 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365739/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 메서드 <a href="#reload-fang-fa-fang-fa" id="reload-fang-fa-fang-fa"></a>

&#x20;  ListView.reload()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365739/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 설명 <a href="#reload-fang-fa-miao-shu" id="reload-fang-fa-miao-shu"></a>

데이터베이스에서 데이터를 다시 로드합니다.

리스트뷰 설정에서 "데이터 새로 고침"을 설정할 수 있으며, 이 옵션을 선택하지 않으면 reload 메서드를 사용하여 데이터베이스에서 데이터를 다시 로드할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365739/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) **매개 변수** <a href="#reload-fang-fa-can-shu-shuo-ming" id="reload-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365739/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) **반환값**  <a href="#reload-fang-fa-fan-hui-zhi" id="reload-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365739/blue%20block.png?version=1\&modificationDate=1648092734000\&api=v2) 예제 <a href="#reload-fang-fa-shi-li" id="reload-fang-fa-shi-li"></a>

다음 예제 코드에서는 reload 메서드를 통해 데이터베이스에서 데이터를 다시 로드합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트 1");
//데이터베이스에서 데이터 다시 로드
listview.reload();
```



#### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. 데이터베이스 테이블을 한 개 생성한 후, 이름/생년월일/부서 열을 생성합니다.\
   데이터는 넣어도 되고 안 넣어도 됩니다. 본 예제에서는 알아보기 쉽게 하기 위해 가짜 데이터를 입력했습니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-reload01.png" alt=""><figcaption></figcaption></figure>

2\. 화면의 영역을 선택하고 “ListView로 설정” 기능을 이용하여, ListView를 생성합니다.\
이 때, 데이터베이스를 선택하라고 나타나는데, 위에서 생성한 테이블을 선택하시면 됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-reload02.png" alt=""><figcaption></figcaption></figure>

3\. ListView에 데이터를 쉽게 입력하는 방법은 아래와 같습니다. 테이블의 열-이름을 드래그하면 됩니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-reload03.gif" alt=""><figcaption></figcaption></figure>

4\. ListView의 이름을 설정합니다. ListView의 이름은 클릭 시 오른쪽의 ‘셀 유형’ 탭에서 나타납니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-reload04.png" alt=""><figcaption></figcaption></figure>

5\. 버튼을 한 개 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령을 이용하여 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-reload05.png" alt=""><figcaption></figcaption></figure>

6\. 프로젝트를 생성합니다. 페이지가 로딩된 후 데이터베이스를 변경합니다.\
프로젝트를 저장하고 다시 웹페이지로 돌아가서 Reload 버튼을 클릭하면 ListView에 새로 입력한 데이터가 나타납니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_listview-reload06.gif)
