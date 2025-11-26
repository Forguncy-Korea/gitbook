# MouseLeave 이벤트

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364848/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 이벤트 <a href="#mouseleave-shi-jian-shi-jian" id="mouseleave-shi-jian-shi-jian"></a>

&#x20;  Forguncy.CellEvents.MouseLeave

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364848/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 설명 <a href="#mouseleave-shi-jian-miao-shu" id="mouseleave-shi-jian-miao-shu"></a>

마우스가 셀을 떠날 때 트리거되며 버튼, 이미지 및 하이퍼링크 셀 유형을 지원합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364848/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) **반환값**  <a href="#mouseleave-shi-jian-fan-hui-zhi" id="mouseleave-shi-jian-fan-hui-zhi"></a>

string

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364848/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 예제 <a href="#mouseleave-shi-jian-shi-li" id="mouseleave-shi-jian-shi-li"></a>

다음 예제 코드에서는 bind 메서드를 사용하여 이미지에 MouseLeave 이벤트를 추가하고 마우스가 이미지셀을 떠날 때 경고 상자가 나타납니다.

```
//CallBack으로 사용할 이벤트를 정의합니다.
  var leavingMouseEvent = function(arg) {
      alert("안녕하세요. Forguncy!");
  }
  
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;

  //Cell Name이 picture라고 되어 있는 셀 인스턴스 속성을 가져옵니다.
  var cell = page.getCell("picture");

  //picture 셀에 leavingMouseEvent 이벤트를 binding합니다.
  cell.bind("mouseLeave", leavingMouseEvent);

  //mouseLeave는 클릭하여 이벤트를 binding해야 실행되는 점 참고하세요.

```

#### Forguncy 사용 예제

1. 페이지 한 개 생성하고, 이미지 셀을 생성하여 그림을 삽입합니다.\
   이후 왼쪽 상단의 Cell Name에 picture라고 입력합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-mouseenter01.png" alt=""><figcaption></figcaption></figure>

2\. 그림 셀을 클릭 후 ‘명령 편집’에서 “자바크스립트로 직접 프로그래밍하기” 명령을 추가하여, 코드를 입력합니다.<br>

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-mouseleave02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하여 나타나는 그림에 마우스 커서를 올려 클릭합니다. 그러면 이벤트가 binding됩니다.\
이후 마우스 커서를 그림 밖으로 옮기면 팝업창이 화면에 표시됩니다.

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-mouseleave03.gif)

<br>
