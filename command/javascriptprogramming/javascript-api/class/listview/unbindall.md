# unbindAll 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365837/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 메서드 <a href="#unbindall-fang-fa-fang-fa" id="unbindall-fang-fa-fang-fa"></a>

&#x20;  ListView.unbindAll()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365837/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 설명 <a href="#unbindall-fang-fa-miao-shu" id="unbindall-fang-fa-miao-shu"></a>

페이지 리스트뷰의 모든 이벤트에 대한 바인딩을 제거합니다. 이 메서드는 페이지 리스트뷰의 모든 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365837/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) **매개 변수** <a href="#unbindall-fang-fa-can-shu-shuo-ming" id="unbindall-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365837/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) **반환값**  <a href="#unbindall-fang-fa-fan-hui-zhi" id="unbindall-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365837/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 예제 <a href="#unbindall-fang-fa-shi-li" id="unbindall-fang-fa-shi-li"></a>

다음 예제 코드에서는 unbindAll 메서드를 사용하여 테이블의 모든 이벤트 바인딩을 제거합니다.

```
//이벤트 핸들러 정의
var onSelectionChanged = function() {
     alert("이동 가능한 타입");
}
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 리스트뷰1이라는 리스트뷰 가져옵니다.
var listivew = page.getListView("리스트뷰1");
//테이블의 이벤트 바인딩
listivew.bind("SelectionChanged", onSelectionChanged);
//모든 이벤트 핸들러 바인딩 해제
listivew.unbindAll();
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365837/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 사용 예제 <a href="#unbindall-fang-fa-shi-li" id="unbindall-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365821/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092736000\&api=v2)디자이너의 페이지에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1343).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365837/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092736000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 클릭한 다음 테이블의 현재 행을 변경하면 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (2064).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365837/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092736000\&api=v2)디자이너에서 버튼을 선택하고 명령을 편집하고 JavaScript 코드에 한 줄의 코드를 추가합니다.

<figure><img src="../../../../../.gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365837/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092736000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 다시 클릭한 후 테이블의 현재 행을 변경하면 경고 상자가 나타나지 않습니다



