# 작업 리스트뷰

현재 페이지로 가져온 후 리스트뷰 이름으로 리스트뷰 개체를 가져오면 리스트뷰의 셀 값을 조작하는 메서드가 포함된 리스트뷰 개체를 조작할 수 있으며 행 변경 이벤트 선택과 같은 이벤트도 사용할 수 있습니다.

리스트뷰  개체를 가져오면 리스트뷰 조작하여 리스트뷰 개체에 대한 여러 가지 방법을 구현할 수 있습니다. 자세한 방법은 ListView 클래스를 참조하십시오.

예를 들어 addNewRow 메서드를 사용하여 리스트뷰에 새 행과 데이터 행을 추가합니다.

```javascript
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 양식 가져오기
var listview = page.getListView("listview1");
//새 줄 추가
listview.addNewRow(
{
"이름": "김남",
"생년월일": new Date(1990, 1, 3),
"부서": "마케팅 부서"
});
```

![](https://help.grapecity.com.cn/download/thumbnails/56532230/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1611021619000\&api=v2) 새 데이터 테이블 직원 테이블을 만들고 이름, 생년월일 및 부서에 세 개의 필드를 추가합니다

<figure><img src="../../.gitbook/assets/image (1517).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532230/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1611021619000\&api=v2) 페이지에서 범위를 선택하고, 데이터 테이블을 셀 범위로 드래그하고, 데이터 테이블의 필드를 바인딩하고, 각 열의 열 이름을 설정합니다.

<figure><img src="../../.gitbook/assets/image (1494).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532230/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021619000\&api=v2) 셀 범위를 선택하고 셀 유형을 버튼을 설정하고 명령을 \[자바스크립트로 직접 프로그래밍하기]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../.gitbook/assets/image (2168).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532230/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021619000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 페이지에서 새 행 추가 버튼을 클릭하면 리스트뷰에 데이터 행이 추가됩니다.

<br>

<figure><img src="../../.gitbook/assets/image (2044).png" alt=""><figcaption></figcaption></figure>

## 리스트뷰 이벤트&#x20;

테이블을 가져온 후 리스트뷰에서 지원하는 이벤트에 대한 [ListViewEvents 클래스](https://help.grapecity.com.cn/pages/viewpage.action?pageId=56533051)를 참조하여 리스트뷰에 이벤트를 바인딩할 수도 있습니다.

예를 들어 bnd 메서드를 사용하면 리스트뷰에 Reloaded 이벤트를 바인딩하고 리스트뷰가 데이터를 다시 로드할 때 경고 상자가 나타납니다.

```javascript
//이벤트 핸들러 정의
var reload = function(arg) {
     alert("이동 가능한 타입");
}
// 현재 페이지 가져오기
var page = Forguncy.Page;
//테이블 객체 가져오기
var listview = page.getListView("리스트뷰1");
//테이블의 이벤트 바인딩
listview.bind("reloaded", reload);
```

![](https://help.grapecity.com.cn/download/thumbnails/56532230/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1611021619000\&api=v2) 페이지에서 범위를 선택하고 데이터 테이블을 셀 범위로 드래그하여 데이터 테이블의 필드를 바인딩합니다.

<figure><img src="../../.gitbook/assets/image (1857).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532230/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1611021619000\&api=v2) 테이블 일정에 따라 데이터를 새로 고치도록 설정합니다. 테이블을 선택하고 마우스 오른쪽 버튼을 클릭한 다음 오른쪽 클릭 메뉴에서 리스트뷰 설정을 선택합니다.

리스트뷰 옵션 대화 상자의 데이터 탭에서 선택 시 자동으로 데이터 다시 불러오기에 체크하고, 간격을 2초로 설정합니다.&#x20;

<figure><img src="../../.gitbook/assets/image (1742).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532230/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021619000\&api=v2) 페이지 설정을 클릭하고 페이지 로드 시 명령을 편집합니다. 명령은 자바스크립트로 직접 프로그래입니다. JavaScript 코드를 입력합니다.

<figure><img src="../../.gitbook/assets/image (2173).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56532230/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021619000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 리스트뷰가 자동으로 새로 고쳐지면 경고창이 나타납니다.

<figure><img src="../../.gitbook/assets/image (328).png" alt=""><figcaption></figcaption></figure>
