# SelectedRowsChanged 이벤트

#### 이벤트 <a href="#selectedrowschanged-shi-jian-shi-jian" id="selectedrowschanged-shi-jian-shi-jian"></a>

&#x20;  Forguncy.ListViewEvents.SelectedRowsChanged

#### 설명 <a href="#selectedrowschanged-shi-jian-miao-shu" id="selectedrowschanged-shi-jian-miao-shu"></a>

&#x20;  이 이벤트는 사용자가 선택 열을 클릭할 때와 같이 리스트뷰의 선택 행이 변경될 때 트리거됩니다. 리스트뷰의 현재 행이 변경될 때만 트리거되는 SelectionChanged 이벤트와 다릅니다.

#### **반환** <a href="#selectedrowschanged-shi-jian-fan-hui-zhi" id="selectedrowschanged-shi-jian-fan-hui-zhi"></a>

&#x20;  string

#### 예제 <a href="#selectedrowschanged-shi-jian-shi-li" id="selectedrowschanged-shi-jian-shi-li"></a>

다음 예제 코드에서는  메서드를 통해 리스트뷰에 SelectedRowsChanged 이벤트를 바인딩하고 리스트뷰의 선택 행이 변경되면 경고 상자가 나타납니다.

```
//이벤트 핸들러 정의
var select = function(arg) {
    alert("이동 가능한 타입);
}
// 현재 페이지 가져오기
var page = Forguncy.Page;
//리스트 객체 가져오기
var listview = page.getListView("리스트뷰1");
//리스트뷰의 이벤트 바인딩
listview.bind("selectedRowsChanged", select);
```

#### &#x20;사용 예제  <a href="#selectedrowschanged-shi-jian-shi-li" id="selectedrowschanged-shi-jian-shi-li"></a>

1. &#x20;페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.
2. &#x20;페이지 설정을 클릭하고 페이지 로드 시 명령을 편집합니다. 명령은 JavaScript 명령입니다. JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1100).png" alt=""><figcaption></figcaption></figure>

3. 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.\
   페이지를 실행하면 기본 테이블에 행이 선택되지 않고 선택 열이 선택되면 경고 상자가 나타납니다.
