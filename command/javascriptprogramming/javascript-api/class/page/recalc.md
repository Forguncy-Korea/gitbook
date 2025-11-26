# recalc 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366172/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 메서드 <a href="#recalc-fang-fa-fang-fa" id="recalc-fang-fa-fang-fa"></a>

page.recalc()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366172/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 설명 <a href="#recalc-fang-fa-miao-shu" id="recalc-fang-fa-miao-shu"></a>

페이지의 모든 수식을 강제로 다시 계산합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366172/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) **매개 변수** <a href="#recalc-fang-fa-can-shu-shuo-ming" id="recalc-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366172/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) **반환값**  <a href="#recalc-fang-fa-fan-hui-zhi" id="recalc-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72366172/blue%20block.png?version=1\&modificationDate=1648092741000\&api=v2) 예제 <a href="#recalc-fang-fa-shi-li" id="recalc-fang-fa-shi-li"></a>

다음 예제 코드에서는 recalc 메서드를 사용하여 페이지의 모든 수식을 강제로 트리거하여 다시 계산합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 강제로 페이지의 모든 수식을 다시 계산하도록 트리거합니다.
page.recalc();
```



#### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, 셀에 =NOW()라고 입력합니다. 해당 함수는 Excel에서 “현재 날짜와 시간”을 표시하는 함수입니다.\
   ※참고 : Forguncy는 Excel에서 사용하는 함수를 사용하여 웹에서 결과를 볼 수 있도록 해 줍니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-recalc01.png" alt=""><figcaption></figcaption></figure>

2\. 버튼을 추가합니다. ‘명령 편집’으로 ‘자바스크립트로 직접 프로그래밍하기’하여 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-recalc02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하여 버튼을 클릭하면 아래와 같이 현재 시간이 변경되어 화면에 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-recalc03.gif)
