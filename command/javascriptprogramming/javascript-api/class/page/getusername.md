# getUserName 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366144/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 메서드 <a href="#getusername-fang-fa-fang-fa" id="getusername-fang-fa-fang-fa"></a>

page.getUserName()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366144/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 설명 <a href="#getusername-fang-fa-miao-shu" id="getusername-fang-fa-miao-shu"></a>

현재 로그인한 사용자의 사용자 이름을 가져오고 사용자가 로그인하지 않은 경우 null 값을 반환합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366144/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) **매개 변수**  <a href="#getusername-fang-fa-can-shu-shuo-ming" id="getusername-fang-fa-can-shu-shuo-ming"></a>

&#x20;  **없음**&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366144/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) **반환값**  <a href="#getusername-fang-fa-fan-hui-zhi" id="getusername-fang-fa-fan-hui-zhi"></a>

string

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366144/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 예제입니다 <a href="#getusername-fang-fa-shi-li" id="getusername-fang-fa-shi-li"></a>

다음 예제 코드에서는 getUserName 메서드를 통해 사용자 이름을 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
//현재 로그인한 사용자의 사용자 이름을 가져옵니다.
var userName = page.getUserName();
//현재 로그인한 사용자의 사용자 이름을 보여주는 경고 상자가 나타납니다.
alert(userName);
```



#### Forguncy 사용 예제

1. 페이지를 생성한 후 셀에 “현재 사용자” 셀 유형을 적용합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getusername01.png" alt=""><figcaption></figcaption></figure>

2\. 해당 페이지에 버튼을 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getusername02.png" alt=""><figcaption></figcaption></figure>

3\. 프로젝트를 실행하여 버튼을 누르면 getUserName을 화면에 표시합니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-getusername03.gif)
