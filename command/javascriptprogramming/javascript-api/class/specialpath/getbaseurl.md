# getBaseUrl 메소드

#### 메서드 <a href="#getbaseurl-fang-fa-fang-fa" id="getbaseurl-fang-fa-fang-fa"></a>

&#x20;  SpecialPath.getBaseUrl()

#### 설명 <a href="#getbaseurl-fang-fa-miao-shu" id="getbaseurl-fang-fa-miao-shu"></a>

응용 프로그램 웹 사이트의 루트 URL을 가져옵니다. 앱이 게시되지 않은 경우 가져온 루트 URL은 "/"입니다.

#### **매개 변수**  <a href="#getbaseurl-fang-fa-can-shu-shuo-ming" id="getbaseurl-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### **반환값** <a href="#getbaseurl-fang-fa-fan-hui-zhi" id="getbaseurl-fang-fa-fan-hui-zhi"></a>

string

#### 예제 <a href="#getbaseurl-fang-fa-shi-li" id="getbaseurl-fang-fa-shi-li"></a>

다음 예제 코드에서는 getBaseUrl 메서드를 사용 하 여 응용 프로그램 웹 사이트의 루트 URL을 가져옵니다.

```
// 도움말 메소드 얻기
var helper = Forguncy.Helper;
// 애플리케이션 웹사이트의 루트 URL을 가져옵니다.
var url = helper.SpecialPath.getBaseUrl();
// 루트 URL을 보여주는 경고 상자 팝업
alert(url);
```

**사용예제**&#x20;

1. 페이지에서 셀 범위를 선택하고, 셀 유형을 버튼으로 설정하고, 명령을 \[자바스크립트로 직접 프로그래밍하]으로 편집하고, JavaScript 코드를 입력합니다.

<figure><img src="../../../../../.gitbook/assets/image (1068).png" alt=""><figcaption></figcaption></figure>

2. 앱을 게시합니다. 리본 메뉴 모음에서 게시-서버를 선택하고 게시 설정 대화 상자에 적절한 매개 변수를 입력한 다음 게시를 클릭합니다.

<figure><img src="../../../../../.gitbook/assets/image (1653).png" alt=""><figcaption></figcaption></figure>

3. 게시 후 앱에 로그인하고 홈 페이지에서 BaseURL 버튼을 클릭하면 앱 웹 사이트의 루트 URL을 표시하는 경고 상자가 나타납니다.

<figure><img src="../../../../../.gitbook/assets/image (418).png" alt=""><figcaption></figcaption></figure>
