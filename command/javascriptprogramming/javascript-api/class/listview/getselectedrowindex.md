# getSelectedRowIndex 메서드

#### 메서드 <a href="#getselectedrowindex-fang-fa-fang-fa" id="getselectedrowindex-fang-fa-fang-fa"></a>

&#x20;  ListView.getSelectedRowIndex()

#### 설명 <a href="#getselectedrowindex-fang-fa-miao-shu" id="getselectedrowindex-fang-fa-miao-shu"></a>

현재 행의 행 인덱스를 가져옵니다. 행 인덱스는 0부터 시작합니다.

#### **매개 변수** <a href="#getselectedrowindex-fang-fa-can-shu-shuo-ming" id="getselectedrowindex-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### **반환값**  <a href="#getselectedrowindex-fang-fa-fan-hui-zhi" id="getselectedrowindex-fang-fa-fan-hui-zhi"></a>

&#x20;  number

#### 예제 <a href="#getselectedrowindex-fang-fa-shi-li" id="getselectedrowindex-fang-fa-shi-li"></a>

다음 예제 코드에서는 getSelectedRowIndex 메서드를 통해 현재 행의 행 인덱스를 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰 1");
//현재 행의 행 인덱스 가져오기
var index = listview.getSelectedRowIndex();
// 현재 행의 행 인덱스를 표시하는 경고 상자 팝업
alert(index);
```

&#x20;**사용 예제**&#x20;

1. 페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.
2. 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1071).png" alt=""><figcaption></figcaption></figure>

3. 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 버튼을 클릭하면 현재 행의 행 인덱스를 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1956).png" alt=""><figcaption></figcaption></figure>
