# SelectionChanged 이벤트

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364875/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 이벤트 <a href="#selectionchanged-shi-jian-shi-jian" id="selectionchanged-shi-jian-shi-jian"></a>

&#x20;  Forguncy.CellEvents.SelectionChanged

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364875/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 설명 <a href="#selectionchanged-shi-jian-miao-shu" id="selectionchanged-shi-jian-miao-shu"></a>

셀의 선택 항목이 변경될 때 이벤트가 트리거됩니다. 콤보 상자 및 사용자 선택 상자 셀 유형을 지원합니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364875/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) **반환값**  <a href="#selectionchanged-shi-jian-fan-hui-zhi" id="selectionchanged-shi-jian-fan-hui-zhi"></a>

&#x20;  string

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364875/blue%20block.png?version=1\&modificationDate=1648092721000\&api=v2) 예제입니다 <a href="#selectionchanged-shi-jian-shi-li" id="selectionchanged-shi-jian-shi-li"></a>

다음 예제 코드에서는 콤보 상자에 SelectionChanged 이벤트를 추가하는 bind 메서드를 사용하여 콤보 상자의 선택 항목이 변경될 때 경고 상자가 나타납니다.

```
 //CallBack으로 사용할 이벤트를 정의합니다.
  var selectionChangedEvent  = function(arg) {
      alert("안녕하세요. Forguncy!");
  }
  
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;

  //Cell Name이 combo라고 되어 있는 셀 인스턴스 속성을 가져옵니다.
  var cell = page.getCell("combo");

  //combo 셀이 변경될 때 selectionChagnedEvent 이벤트를 binding합니다.
  cell.bind("selectionChanged", selectionChangedEvent);
```



#### Forguncy 사용 예제

1. 페이지 한 개 생성하고, 콤보박스 셀을 생성합니다. 이후 왼쪽 상단의 Cell Name에 combo라고 입력합니다.\
   그런 다음 콤보박스 셀을 선택하고 오른쪽에 콤보박스에 나타날 값들을 입력해줍니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-selectionchanged01.png" alt=""><figcaption></figcaption></figure>

2\. 콤보박스 셀을 클릭 후 ‘명령 편집’에서 “자바크스립트로 직접 프로그래밍하기” 명령을 추가하여, 코드를 입력합니다.

<figure><img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-selectionchanged02.png" alt=""><figcaption></figcaption></figure>

3\. 해당 프로젝트를 실행하여 나타나는 콤보박스의 값을 변경합니다. 첫 번 째 변경에 이벤트가 binding되고, 두 번 째 변경부터는 이벤트가 실행됩니다.<br>

![](https://forguncy-korea.github.io/images/forguncy5/ex-ss_cellevent-selectionchanged03.gif)
