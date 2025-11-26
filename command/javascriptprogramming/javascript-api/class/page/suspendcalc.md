# suspendCalc 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366240/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 메서드 <a href="#suspendcalc-fang-fa-fang-fa" id="suspendcalc-fang-fa-fang-fa"></a>

&#x20;  Page.suspendCalc()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366240/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 설명 <a href="#suspendcalc-fang-fa-miao-shu" id="suspendcalc-fang-fa-miao-shu"></a>

일시 중단된 페이지의 수식 계산 논리, 즉 페이지의 수식 계산을 일시 중지합니다. 일반적으로 더 나은 성능을 위해 셀 값을 많이 조작하기 전에 사용됩니다. 복구 계산은 [resumeCalc 메서드](resumecalc.md)를 사용합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366240/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) **매개 변수** <a href="#suspendcalc-fang-fa-can-shu-shuo-ming" id="suspendcalc-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366240/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) **반환값**  <a href="#suspendcalc-fang-fa-fan-hui-zhi" id="suspendcalc-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366240/blue%20block.png?version=1\&modificationDate=1648092742000\&api=v2) 예제 <a href="#suspendcalc-fang-fa-shi-li" id="suspendcalc-fang-fa-shi-li"></a>

다음 예제 코드에서는 suspendCalc 메서드를 사용하여 페이지의 모든 수식을 일시 중단하고 계산하지 않습니다.

```
//현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지에서 수식 계산을 일시 중지합니다.
page.suspendCalc();
```



#### Forguncy 사용 예제

※알림: 아래 사용 예제는 [suspendCalc](https://forguncy-korea.github.io/fgc5jsapi_page-class-suspendcalc.html)와 [resumeCalc](https://forguncy-korea.github.io/fgc5jsapi_page-class-resumecalc.html)를 동시에 사용하므로, 같은 예제를 사용합니다.

1. 페이지를 한 개 생성하고, 셀 영역을 선택하여 “텍스트 상자”를 생성합니다.

\
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-resumecalc01.png" alt=""><figcaption></figcaption></figure>

2\. 텍스트 상자 아래 쪽에 병합 셀을 하나 생성하고, 위에서 생성한 텍스트 상자를 참조하도록 합니다. (화면에서 =B2로 표현되어 있습니다.)

\
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-resumecalc02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하면 입력 박스 하나와 숫자 0이 나타납니다. 해당 입력 박스에 아무거나 입력 후 Enter키를 누르면 숫자 0은 입력한 대로 표시됩니다.

\
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-resumecalc03.png" alt=""><figcaption></figcaption></figure>

4\. Forguncy Editor로 돌아가 버튼을 한 개 생성하고, “자바스크립트로 직접 프로그래밍하기” 명령을 생성하여 코드를 입력합니다.

\
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-resumecalc04.png" alt=""><figcaption></figcaption></figure>

5\. 다시 해당 프로젝트를 실행한 후 “버튼”을 클릭합니다. 이후 입력 창에 아무거나 입력 후 Enter키를 눌러 봅니다. 값이 변경되지 않으면 suspendCalc가 잘 적용된 것입니다.

\
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-resumecalc05.png" alt=""><figcaption></figcaption></figure>

6\. 다시 Forguncy Editor로 돌아가 버튼을 한 개 더 생성하고, 명령을 생성하여 코드를 입력합니다.

\
<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-resumecalc06.png" alt=""><figcaption></figcaption></figure>

7\. 다시 한 번 해당 프로젝트를 생성하고, 다음의 방법으로 테스트를 진행합니다.\
(1) suspendCalc를 적용한 버튼을 클릭합니다.\
(2) 입력 상자에 아무거나 입력 후 Enter키를 누릅니다. ▶ 값이 변하지 않으면 성공입니다.\
(3) resumeCalc를 적용한 버튼을 클릭합니다.\
(4) 입력 상자에 아무거나 입력 후 Enter키를 누릅니다. ▶ 값이 입력한 대로 변하면 성공입니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-resumecalc07.gif)
