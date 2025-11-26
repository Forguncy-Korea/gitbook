# getContentPage 메서드

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364992/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) 메서드 <a href="#getcontentpage-fang-fa-fang-fa" id="getcontentpage-fang-fa-fang-fa"></a>

&#x20;  Cell.getContentPage()

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364992/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) 설명 <a href="#getcontentpage-fang-fa-miao-shu" id="getcontentpage-fang-fa-miao-shu"></a>

페이지 컨테이너의 자식 페이지 개체를 가져옵니다. 이 메서드는 셀 유형이 페이지 컨테이너인 경우에만 사용할 수 있습니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364992/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) **매개 변수**  <a href="#getcontentpage-fang-fa-can-shu-shuo-ming" id="getcontentpage-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364992/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) **값을 반환합니다** <a href="#getcontentpage-fang-fa-fan-hui-zhi" id="getcontentpage-fang-fa-fan-hui-zhi"></a>

&#x20;  SubPage

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364992/blue%20block.png?version=1\&modificationDate=1648092723000\&api=v2) 예제입니다 <a href="#getcontentpage-fang-fa-shi-li" id="getcontentpage-fang-fa-shi-li"></a>

다음 예제 코드에서는 getContentPage 메서드를 사용하여 지정된 페이지 컨테이너(container)의 하위 페이지(페이지 1)의 셀(myCell) 값을 가져옵니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 페이지 컨테이너 가져오기
var containerCell = page.getCell("container");
//페이지 컨테이너의 자식 페이지 가져오기
var subPage = containerCell.getContentPage();
// 하위 페이지의 이름이 페이지 1인지 확
if (subPage.getPageName() == "页面1") {
//하위 페이지의 셀 가져오기
var subPageCell = subPage.getCell("myCell");
};
// 셀의 값을 가져오고 경고 상자를 표시합니다.
alert(subPageCell.getValue());
```



#### Forguncy 사용 예제

1. 페이지를 두 개 생성합니다. 첫 번 째 페이지에는 “내용이 포함된 셀”을 선택합니다.\
   화면 왼쪽 상단의 Cell Name에 container라고 이름을 붙여줍니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getcontainerpage01.png" alt=""><figcaption></figcaption></figure>

2\. 두 번 째 페이지에는 컨텐츠를 넣어 줍니다. 예제에서는 화면 내 결과 출력을 위해 텍스트를 입력했습니다.\
이후 페이지 왼쪽 위에 해당 Cell Name을 myCell이라고 적어줍니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getcontainerpage02.png" alt=""><figcaption></figcaption></figure>

3\. 다시 첫 번 째 페이지로 가시 “내용이 포함된 셀”에 두 번 째 페이지를 넣어 줍니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getcontainerpage03.png" alt=""><figcaption></figcaption></figure>

4\. 페이지에 버튼을 하나 생성하고, 해당 버튼에 “자바스크립트로 직접 프로그래밍하기” 명령으로 코드를 입력합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getcontainerpage04.png" alt=""><figcaption></figcaption></figure>

5\. 해당 프로젝트를 실행하고 버튼을 클릭하면 하위 페이지의 myCell에 들어 있는 테스트 값이 화면에 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cell-getcontainerpage05.gif)
