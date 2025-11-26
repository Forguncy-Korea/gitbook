# bind 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365423/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 메서드 <a href="#bind-fang-fa-fang-fa" id="bind-fang-fa-fang-fa"></a>

&#x20;  ListView.bind(type, data, fn)

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365423/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 설명 <a href="#bind-fang-fa-miao-shu" id="bind-fang-fa-miao-shu"></a>

&#x20;  선택한 리스트뷰에 하나 이상의 이벤트 처리기를 추가하고 이벤트가 발생할 때 실행되는 함수를 지정합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365423/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **매개 변수**  <a href="#bind-fang-fa-can-shu-shuo-ming" id="bind-fang-fa-can-shu-shuo-ming"></a>

<table><thead><tr><th width="142">매개변수 </th><th width="141">형식 </th><th width="169">필수여부</th><th>설명 </th></tr></thead><tbody><tr><td>type</td><td>string</td><td>Yes</td><td>이벤트 형식을 나타내는 문자열입니다. 리스트뷰에서 지원되는 이벤트는 ListViewEvents 클래스 를 참조하십시오.</td></tr><tr><td>data</td><td>any</td><td>No</td><td>이벤트 처리기에 전달된 사용자 지정 매개 변수를 무시하지 않는 경우 선택적 매개 변수입니다.</td></tr><tr><td>fn</td><td>function</td><td>Yes</td><td>이벤트 처리기입니다.</td></tr></tbody></table>

<br>

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365423/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) **반환값**  <a href="#bind-fang-fa-fan-hui-zhi" id="bind-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365423/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 예제 <a href="#bind-fang-fa-shi-li" id="bind-fang-fa-shi-li"></a>

다음 예제 코드에서는 bind 메서드를 사용하여 리스트뷰에 현재 행 변경 이벤트 처리기를 추가하고 리스트뷰의 현재 행이 변경될 때 경고 상자가 나타납니다.

```
// 이벤트 핸들러에 사용자 정의 매개변수를 전달할 필요가 없습니다.
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 페이지에서 리스트뷰 1이라는 리스트뷰를 가져옵니다.
var listview = page.getListView("리스트1");
//리스트뷰의 이벤트 바인딩
listview.bind("SelectionChanged", function () {
    alert("이동 가능한 타입");
});
```

#### ![](https://help.grapecity.com.cn/download/thumbnails/72365423/blue%20block.png?version=1\&modificationDate=1648092729000\&api=v2) 사용 예제  <a href="#bind-fang-fa-shi-li" id="bind-fang-fa-shi-li"></a>

![](https://help.grapecity.com.cn/download/thumbnails/72365423/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092729000\&api=v2)페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 각 열의 열 이름을 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72365423/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092729000\&api=v2)페이지 설정에서 \[페이지 로드 시 명령 편집]을 클릭하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1656).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72365423/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092729000\&api=v2)편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 테이블의 현재 행을 변경하면 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1619).png" alt=""><figcaption></figcaption></figure>
