# unbind 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365821/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 메서드 <a href="#unbind-fang-fa-fang-fa" id="unbind-fang-fa-fang-fa"></a>

&#x20;  ListView.unbind(type, fn)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365821/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 설명 <a href="#unbind-fang-fa-miao-shu" id="unbind-fang-fa-miao-shu"></a>

선택한 리스트뷰에 대한 이벤트 처리기를 제거합니다. 이 메서드는 선택한 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365821/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) **매개 변수**  <a href="#unbind-fang-fa-can-shu-shuo-ming" id="unbind-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="154">매개변수</th><th width="144">유형 </th><th width="134">필수여부 </th><th>설명 </th></tr></thead><tbody><tr><td>type</td><td>string</td><td>YES</td><td>이벤트 형식을 나타내는 문자열입니다. 리스트뷰에서 지원되는 이벤트는 ListViewEvents 클래스 를 참조하십시오.</td></tr><tr><td>fn</td><td>function</td><td>NO</td><td>이벤트 처리기입니다. 생략하면 리스트뷰에서 해당 이벤트 형식의 모든 처리기가 바인딩 해제됩니다.</td></tr></tbody></table>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365821/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) **반환값**  <a href="#unbind-fang-fa-fan-hui-zhi" id="unbind-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365821/blue%20block.png?version=1\&modificationDate=1648092736000\&api=v2) 예제 <a href="#unbind-fang-fa-shi-li" id="unbind-fang-fa-shi-li"></a>

다음 예제 코드에서 unbind 메서드를 사용 하 여 리스트뷰에 대 한 이벤트 바인딩을 제거 합니다.

```
//이벤트 핸들러 정의
var onSelectionChanged = function () {
    alert("이동 가능한 타입");
}
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 리스트뷰 1이라는 리스트뷰를 가져옵니다.
var listivew = page.getListView("리스트뷰1");
//리스트의 이벤트 바인딩
listivew.bind("SelectionChanged", onSelectionChanged);
//특정 이벤트 핸들러 바인딩 해제 
listivew.unbind("SelectionChanged", onSelectionChanged);
```

![](https://help.grapecity.com.cn/download/thumbnails/72365821/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092736000\&api=v2)디자이너의 페이지에서 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1384).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365821/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092736000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼 클릭한 다음 테이블의 현재 행을 변경하면 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (2064).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365821/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092736000\&api=v2)디자이너에서 버튼을 선택하고 명령을 편집하고 JavaScript 코드에 한 줄의 코드를 추가합니다.

<figure><img src="../../../../../.gitbook/assets/image (1286).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365821/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092736000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 다시 클릭한 후 테이블의 현재 행을 변경하면 경고 상자가 나타나지 않습니다.
