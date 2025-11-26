# Reloaded 이벤트

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365326/blue%20block.png?version=1\&modificationDate=1648092728000\&api=v2) 이벤트 <a href="#reloaded-shi-jian-shi-jian" id="reloaded-shi-jian-shi-jian"></a>

&#x20;  Forguncy.ListViewEvents.Reloaded

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365326/blue%20block.png?version=1\&modificationDate=1648092728000\&api=v2) 설명 <a href="#reloaded-shi-jian-miao-shu" id="reloaded-shi-jian-miao-shu"></a>

이 이벤트는 리스트뷰 데이터를 다시 로드할 때 트리거됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365326/blue%20block.png?version=1\&modificationDate=1648092728000\&api=v2) **반환값**  <a href="#reloaded-shi-jian-fan-hui-zhi" id="reloaded-shi-jian-fan-hui-zhi"></a>

&#x20;  string

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365326/blue%20block.png?version=1\&modificationDate=1648092728000\&api=v2) 예제 <a href="#reloaded-shi-jian-shi-li" id="reloaded-shi-jian-shi-li"></a>

다음 예제 코드에서는  메서드를 통해 리스트에 Reloaded 이벤트를 바인딩하고 리스트뷰 데이터를 다시 로드할 때 경고 상자가 나타납니다.

```
//이벤트 핸들러 정의
var reload = function(arg) {
    alert("이동 가능한 타입");
}
// 현재 페이지 가져오기
var page = Forguncy.Page;
//리스트 객체 가져오기
var listview = page.getListView("리스트뷰1");
//리스트뷰의 이벤트 바인딩
listview.bind("reloaded", reload);
```

\
![](https://help.grapecity.com.cn/download/thumbnails/72365326/16.png?version=1\&modificationDate=1648092728000\&api=v2) **사용 예제**&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72365326/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092728000\&api=v2) 페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

<figure><img src="../../../../../.gitbook/assets/image (2158).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365326/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092728000\&api=v2) 리스트뷰를 일정에 따라 데이터를 새로 고치도록 설정합니다.리스트뷰를 선택하고 마우스 오른쪽 버튼을 클릭한 다음 오른쪽 클릭 메뉴에서 리스트뷰 세부 옵션 설정을 선택합니다.

리스트뷰 옵 설정 대화 상자의 데이터 탭에서 선택 시 데자동으로 데이터 다시 불러오기를 선택하고 간격을 설정합니다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (778).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365326/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092728000\&api=v2) 페이지 설정을 클릭하고 페이지 로드 시 명령을 편집합니다. 명령은 JavaScript 명령입니다. JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (892).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365326/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092728000\&api=v2) 페이지를 실행하고 테이블이 자동으로 새로 고쳐지면 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (598).png" alt=""><figcaption></figcaption></figure>
