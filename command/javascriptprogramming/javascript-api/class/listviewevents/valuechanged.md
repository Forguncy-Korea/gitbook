# ValueChanged 이벤트

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365375/blue%20block.png?version=1\&modificationDate=1648092728000\&api=v2) 이벤트 <a href="#valuechanged-shi-jian-shi-jian" id="valuechanged-shi-jian-shi-jian"></a>

&#x20;  Forguncy.ListViewEvents.ValueChanged

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365375/blue%20block.png?version=1\&modificationDate=1648092728000\&api=v2) 설명 <a href="#valuechanged-shi-jian-miao-shu" id="valuechanged-shi-jian-miao-shu"></a>

리스트뷰의 값이 변경될 때 이벤트가 트리거됩니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365375/blue%20block.png?version=1\&modificationDate=1648092728000\&api=v2) **반환값**  <a href="#valuechanged-shi-jian-fan-hui-zhi" id="valuechanged-shi-jian-fan-hui-zhi"></a>

&#x20;  string

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365375/blue%20block.png?version=1\&modificationDate=1648092728000\&api=v2) 예제 <a href="#valuechanged-shi-jian-shi-li" id="valuechanged-shi-jian-shi-li"></a>

다음 예제 코드에서는 메서드를 사용하여 테이블에 ValueChanged 이벤트를 바인딩하고 테이블 값이 변경될 때 경고 상자가 나타납니다.

```
//이벤트 핸들러 정의
var change = function(arg) {
    alert("이동 가능한 타입");
}
/// 현재 페이지 가져오기
var page = Forguncy.Page;
//리스트 객체 가져오기
var listview = page.getListView("리스트뷰1");
//리스트뷰의 이벤트 바인딩
listview.bind("valueChanged", change);
```

#### 사용 예제  <a href="#valuechanged-shi-jian-shi-li" id="valuechanged-shi-jian-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365375/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092729000\&api=v2)페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 테이블의 편집 허용을 켭니다.

<figure><img src="../../../../../.gitbook/assets/image (665).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365375/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092728000\&api=v2)페이지 설정을 클릭하고 페이지 로드 시 명령을 편집합니다. 명령은 JavaScript 명령입니다. JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (556).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365375/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092728000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 테이블의 값을 변경하면 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (2159).png" alt=""><figcaption></figcaption></figure>
