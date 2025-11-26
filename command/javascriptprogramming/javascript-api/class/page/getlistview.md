# getListView 메서드

#### Page - getListView Method

Page.getListViews(name, includeSubPage)\
<br>

#### getListView Method 설명

화면에 보이는 ListView 중 하나의 이름을 기반으로 하여 해당 ListView 인스턴스의 속성을 가져옵니다.\
<br>

#### Parameter 설명

<table><thead><tr><th width="167">매개변수 </th><th width="127">타입</th><th width="115">필수</th><th>상세 설명</th></tr></thead><tbody><tr><td>name</td><td>string</td><td>예</td><td>ListView의 이름을 입력합니다.</td></tr><tr><td>includeSubPage</td><td>boolean</td><td>아니오</td><td>페이지 내 하위 페이지를 포함하는 컨테이너 또는 탭컨트롤이 존재하는 경우 하위 페이지까지 검색할 지 여부를 결정합니다.<br>기본값은 True이며 의미는 “검색함”입니다. False는 “검색하지 않음”입니다.</td></tr></tbody></table>

<br>

#### Response 시 반환값

ListView 속성을 반환합니다. 자세한 내용은 ListView\[]를 참고하세요.

> 😄 ListView Method 관련 내용은 준비 중입니다.

#### 활용 예제

아래는 page.getListViews를 사용하는 관련 사용 예제입니다. 페이지 내 Cell 중 컨테이너 유형의 Cell 인스턴스들의 정보를 불러옵니다.<br>

```
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;

  //이름이 ListView1이라는 ListView의 인스턴스를 가져옵니다.
  var listview = page.getListView("ListView1");

  //ListView1의 속성 중 이름을 확인합니다.
  var name = listview.getName();
  
  //ListView1의 이름을 화면에 표시합니다.
  alert(name);
```

<br>

#### Forguncy 사용 예제

1.  페이지를 한 개 생성하여 Database Table을 연결하는 ListView를 생성합니다.\
    해당 ListView의 이름을 ListView1이라고 입력합니다.<br>

    <figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getlistview01.png" alt=""><figcaption></figcaption></figure>
2.  해당 페이지에 버튼을 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 추가합니다.<br>

    <figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getlistview02.png" alt=""><figcaption></figcaption></figure>
3.  프로젝트를 실행하여 버튼을 누르면 getListView에서 화면의 ListView 인스턴스의 속성 중 이름을 화면에 표시합니다.

    ![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getlistview03.gif)

<br>
