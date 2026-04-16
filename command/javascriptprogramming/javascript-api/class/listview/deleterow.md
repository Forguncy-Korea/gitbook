# deleteRow 메서드

#### 메서드 <a href="#deleterow-fang-fa-fang-fa" id="deleterow-fang-fa-fang-fa"></a>

&#x20;  ListView.deleteRow(rowIndex)

#### 설명 <a href="#deleterow-fang-fa-miao-shu" id="deleterow-fang-fa-miao-shu"></a>

리스트뷰에 지정된 행을 삭제합니다.

#### **매개 변수** <a href="#deleterow-fang-fa-can-shu-shuo-ming" id="deleterow-fang-fa-can-shu-shuo-ming"></a>

| 매개변수     | 형식     | 설명                 |
| -------- | ------ | ------------------ |
| rowIndex | number | 0부터 시작하는 행 인덱스입니다. |

#### **반환값**  <a href="#deleterow-fang-fa-fan-hui-zhi" id="deleterow-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### 예제 <a href="#deleterow-fang-fa-shi-li" id="deleterow-fang-fa-shi-li"></a>

다음 예제 코드에서는 deleteRow 메서드를 사용 하 여 리스트에 지정 된 행을 제거 합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 리스트 가져오기
var listview = page.getListView("리스트뷰1");
// 지정된 줄 삭제
listview.deleteRow(1);
```

#### &#x20;사용 예제  <a href="#deleterow-fang-fa-shi-li" id="deleterow-fang-fa-shi-li"></a>

1. 페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.
2. 셀 범위를 선택하고 셀 유형을 버튼으로 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (697).png" alt=""><figcaption></figcaption></figure>

\
3\. 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.\
페이지를 실행하고 페이지에서 삭제 버튼을 클릭하면 두 번째 행이 삭제됩니다.

<figure><img src="../../../../../.gitbook/assets/image (583).png" alt=""><figcaption></figcaption></figure>
