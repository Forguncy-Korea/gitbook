# getDataTableName 메서드

#### 메서드 <a href="#getdatatablename-fang-fa-fang-fa" id="getdatatablename-fang-fa-fang-fa"></a>

&#x20;  ListView.getDataTableName()

#### 설명 <a href="#getdatatablename-fang-fa-miao-shu" id="getdatatablename-fang-fa-miao-shu"></a>

리스트뷰 바인딩된 데이터 테이블 또는 뷰의 이름을 가져옵니다.

#### **매개 변수**  <a href="#getdatatablename-fang-fa-can-shu-shuo-ming" id="getdatatablename-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### **반환값**  <a href="#getdatatablename-fang-fa-fan-hui-zhi" id="getdatatablename-fang-fa-fan-hui-zhi"></a>

&#x20;  string

#### 예제 <a href="#getdatatablename-fang-fa-shi-li" id="getdatatablename-fang-fa-shi-li"></a>

다음 예제 코드에서는 getDataTableName 메서드를 사용하여 리스트에 바인딩된 데이터 테이블 또는 뷰의 이름을 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
//리스트뷰에 바인딩된 데이터 테이블 또는 뷰의 이름을 가져옵니다.
var name = listview.getDataTableName();
// 데이터 테이블 또는 뷰의 이름을 보여주는 팝업
alert(name);
```

#### 사용 예제 <a href="#getdatatablename-fang-fa-shi-li" id="getdatatablename-fang-fa-shi-li"></a>

1. 페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.
2. 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (384).png" alt=""><figcaption></figcaption></figure>

3. 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.\
   페이지를 실행하고 페이지에서 테이블 이름 가져오기 버튼을 클릭하면 테이블 바인딩된 데이터 테이블 이름을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (1836).png" alt=""><figcaption></figcaption></figure>
